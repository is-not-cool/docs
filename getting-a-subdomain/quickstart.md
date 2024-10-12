# 🏃‍♂️ quickstart

<figure><img src="../.gitbook/assets/5E11EFD0-4C27-429D-83B9-6EA75D3BD429.jpeg" alt=""><figcaption></figcaption></figure>

first, fork the repository as shown in the photo above this text.

{% hint style="info" %}
want to learn how to make your own? buy ur own domain&#x20;
{% endhint %}

### setting up

to set up, you will need to make a json file in the "domains" folder, you will need to make sure it follows this format in json and goes like "yoursubdomain".is-not.cool.json

```
{
    "description": "insert ur description",

    "domain": "is-not.cool",
    "subdomain": "yoursubdomain",

    "owner": {
        "repo": "https://github.com/is-not-cool/registration",
        "email": "ur email adress"
    },

    "record": {
        // choose any dns record that exists and we can try to make it happen
    },

    "proxied": false
}
```



###
