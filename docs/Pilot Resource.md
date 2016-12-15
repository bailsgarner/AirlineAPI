---
layout: page
Title: Pilot Resource
permalink: /Pilotresource/  
---  

# Overview  
The Pilot Resource allows the user to receive information regarding a specific pilot.   

# Functions
The functions of this resource are as follows: 
-
-
-
-
-
-


#### Methods

| Method | Comments |
|--------|----------|
| GET | Returns the specified pilot resource. |
| POST | Adds a new pilot to an airline. |
| PUT | **Not implemented** |
| DELETE | Removes a pilot from an airline. |

#### URL

```
http://<server>/api/pilot/<id>
```

ID = the numeric ID of the pilot

#### Request

| Method | Request info |
|--------|----------|
| GET | The pilot to retrieve is specified by ID in the URL. |
| POST | The pilot is described by a data object that contains the pilot's **LastName**, **FirstName**, & **irlineId** |
| PUT | **Not implemented** |
| DELETE | The pilot to remove is specified by ID in the URL.  |

#### Response

This is a sample response to a pilot request.

```javascript
{
    "PilotId": "1",
    "LastName": "Watson",
    "FirstName": "Bob",
    "AirlineId": "1"
}
```

### scheduledFlight

An instance of a flight that is scheduled for a specific date. The desecription of a **scheduledFlight** refers to a:

* **flight**
* **pilot**
* **plane**


