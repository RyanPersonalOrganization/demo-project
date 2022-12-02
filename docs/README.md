---
tags: [Guides]
---

# Welcome to V2!

</br>
<span style="font-size: 3em; color: #5D535E;">
  <i class="fas fa-robot fa-2x"></i> <i>Robot Factory
</i></span> 
</br>
</br>

[local link](docs/Guides/Best-Practices.md)

[local link 2](devices.v2.yaml/paths/~1api~1myDevices)

[**Backed By This GIT Repo!**](https://github.com/stoplightio/stoplight-platform-demo)

[Stoplight Flavoured Markdown](https://meta.stoplight.io/docs/studio/docs/Documentation/03a-stoplight-flavored-markdown.md)

---

Interact with the `'Devices'` API to get a list of registered devices, add or remove devices and to update existing records.

Use this API to leverage **_Robot Factory_**'s central repository of devices that allows users to manage automation systems at home, at work or on the go.
</br>

<ul class="fa-ul" style="list-style-type:none;">
  <li><span class="fa-li"><i class="fas fa-check-square"></i></span>Register a device</li>
  <li><span class="fa-li"><i class="fas fa-check-square"></i></span>Apply custom runtime settings</li>
  <li><span class="fa-li"><i class="fas fa-check-square"></i></span>Sync devices</li>
  <li><span class="fa-li"><i class="far fa-square"></i></span>Invite friends to <strong>Robot Factory<strong></li>
</ul>

### Code Generation

**Robot Factory**'s API documentation provides code generation to get your project started as soon as you imagine it!

```javascript
var data = null;

var xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://robotfactory.io/api/devices/123?spaceid=all&sort=desc&limit=10");
xhr.setRequestHeader("deviceid", "all");
xhr.setRequestHeader("apikey", "123");

xhr.send(data);
```

> **_Robot Factory_** is the world's best IoT robot developer. Our `API`s are just as great as our user-friendly UI, making us the first choice for systems integrators around the world. Bring the power of IOT to your life with **_Robot Factory_**.

### Interactive Documentation

With the `'Try It!'` functionality you can send requests directly to our servers provided that you have a valid account and **Robot Factory Key**, if you are not an existing customer you can use the built-in mock server for free! Click `'Send'` in the embedded _**Request Maker**_ below to get a sample mocked response:

```json http
{
  "method": "get",
  "url": "https://learning.stoplight.io/mocks/apiguild/robotfactory/30785/api/devices/abc",
  "query": {
    "spaceid": "all",
    "sort": "desc",
    "limit": "10"
  },
  "headers": {
    "deviceid": "all",
    "apiKey": "123",
    "Prefer": "code=200, example=devices"
  }
}
```

### Data Models

If you want to learn more about the data models used by our `APIs`, you can find them at the bottom of the left-hand navigation. Here is an example:
</br>


```json json_schema
{
  "title": "User",
  "type": "object",
  "properties": {
    "id": {
      "type": "string"
    },
    "name": {
      "type": "string",
      "description": "The user's full name."
    },
    "age": {
      "type": "number",
      "minimum": 0,
      "maximum": 150
    },
    "location": {
      "$ref": "../device.v1.json"
    }
  },
  "required": ["id", "name"]
}
```
