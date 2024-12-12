# 🏃‍♂️ Quickstart

<figure><img src="../.gitbook/assets/quickstart.png" alt=""><figcaption></figcaption></figure>

You will need to fork the repository, as shown in the image above.

{% hint style="info" %}
This is a really easy-to-use subdomain service! &#x20;
{% endhint %}

### Setting up

You can get your subdomain from is-not.cool by using the format below, and making the file name be following the of "yoursubdomain".json.

```
{
    "description": "insert ur description",
    "owner": {
        "repo": "https://github.com/is-not-cool/registration",
        "email": "Your email address (If you care about your privacy, you do not have to do this.)",
        "discord": "Your discord ID"
    },

    "record": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["2606:4700:4700::1111", "2606:4700:4700::1001"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "NS": ["ns1.example.com", "ns2.example.com"],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ]
    },

    "proxied": false
}
```
{% hint style="warning" %}
Only select the records you need, Remove the other ones as it may cause errors in the .json file.
{% endhint %}
