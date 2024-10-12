---
label: DanBot Hosting
tags: guides
icon: /img/dbh.jpeg
---

# Setting up DanBot Hosting with is-a.dev subdomain

This guide will walk you through the process of setting up a DanBot Hosting site and pointing your is-a.dev subdomain to it.


## Getting Proxy IP
Execute the following command in [DanBot Hosting Discord server](https://discord.gg/dbh) in the #commands channel.
```
dbh!server proxy
```

You will get a reply like this:


![1](../img/DBH_PROXY_1.jpg)

If you are on free plan, choose any US proxy or you can use the Donator Proxy If you are a Donator, then note the IP address of the proxy you chose.

### Creating the domain file
Create a JSON file inside `domains` directory (`domains/<subdomain>.json`) with the following content and submit a pull request:
```json 
{
    "description": "Describe the use of this subdomain",
    "repo": "https://github.com/<github-username>/<github-repository>",
    "owner": {
        "username": "<github-username>",
        "email": "<email@address>",
        "twitter": "<twitter-username>"
    },
    "record": {
        "A": [
            "proxy-ip-here"
        ]
    }
} 
```
**Note:** In the owner section, you can add any social media handle, such as Discord. If you add another social media account, you can omit the email and Twitter fields. However, the GitHub username is mandatory. Don't forget to provide a preview of your site in your pull request.

## Configuring
After the pull request is merged, get your server ID by running this command:
```
dbh!server list
```

You will get a reply like this:

![2](../img/DBH_PROXY_2.jpg)

Note down the server ID, then execute following command:
```
dbh!server proxy your-subdomain.is-a.dev yourserverid
```
