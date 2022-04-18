---
tags: [requirements, CheckOut]
---

# API Requirements

[Stoplight Flavoured Markdown](https://meta.stoplight.io/docs/studio/docs/Documentation/03a-stoplight-flavored-markdown.md)

## Why 

This API provides an interface for clients to manage robot devices.  This interface can be used from either a mobile or web interface.

## User Stories

-   As a client, I want to list all of my devices 
-   As a client, I want to get information about a specific device
-   As a client, I want to delete a device from the database
-   As a client, I want to update a device

## Data Model

```json
{
  "deviceID": "string",
  "deviceName": "string",
  "deviceClass": "string",
  "spaceID": "string",
  "alexaCompatible": true,
  "storageUsed": 0,
  "storageFree": 0,
  "dateCreated": "2017-07-21T17:32:28Z",
  "dateUpdated": "2017-07-21T17:32:28Z"
}
```

## Wireframe

![Sample Wireframe]()

## Requirements

Extended Requirements