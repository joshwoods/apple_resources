

- Device Management
-  Get the Location of a Device 

Web Service Endpoint

# Get the Location of a Device

Request the location of a device when in Lost Mode.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeviceLocationCommand
```

## HTTP Body

DeviceLocationCommand

The command to request a device’s location.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeviceLocationResponse

`OK`

A response from the device after it processes the command to request its location.

Content-Type: application/xml

## Discussion

A device responds with error code `12067` if it isn’t in Lost Mode, or error code `12068` if its location is unknown. While in Lost Mode, a device responds to invalid commands with error code `12078`.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Requires Supervision       | iOS              |
| Allowed in User Enrollment | \-               |
| Required Access Right      | \-               |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        DeviceLocation

    CommandUUID
    0001_DeviceLocation

```

```

    Altitude
    -1.0
    CommandUUID
    0246_DeviceLocation
    Course
    -1.0
    HorizontalAccuracy
    3.677859038862057
    Latitude
    37.33385013244351
    Longitude
    -122.01079213269968
    Speed
    -1.0
    Status
    Acknowledged
    Timestamp
    2019-09-04T22:35:52Z
    UDID
    00008020-000915083C80012E
    VerticalAccuracy
    -1.0

```

## Topics

### Command and Response

object DeviceLocationCommand

The command to request a device’s location.

object DeviceLocationResponse

A response from a device in Lost Mode after it processes the command to request its location.

## See Also

### Lost Device

Enable Lost Mode

Enable Lost Mode on a device, which provides a message and phone number on the Lock screen.

Play the Lost Mode Sound

Play the Lost Mode sound on a device that’s in Lost Mode.

Disable Lost Mode

Take the device out of Lost Mode.

