

- Device Management
-  Disable Lost Mode 

Web Service Endpoint

# Disable Lost Mode

Take the device out of Lost Mode.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DisableLostModeCommand
```

## HTTP Body

DisableLostModeCommand

The command to disable Lost Mode.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DisableLostModeResponse

`OK`

A response from the device after it processes the command to disable Lost Mode.

Content-Type: application/xml

## Discussion

A device responds with error code `12067` if it isn’t in Lost Mode, or error code `12069` if the request to disable Lost Mode failed. While in Lost Mode, a device responds to invalid commands with error code `12078`.

Erasing a device also disables Lost Mode. To reenable Lost Mode, the MDM server stores the device’s Lost Mode state before erasing it, and restores that state if the device enrolls again.

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
        DisableLostMode

    CommandUUID
    0001_DisableLostMode

```

```

    CommandUUID
    0001_DisableLostMode
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object DisableLostModeCommand

The command to disable Lost Mode.

object DisableLostModeResponse

A response from the device after it processes the command to disable Lost Mode.

## See Also

### Lost Device

Enable Lost Mode

Enable Lost Mode on a device, which provides a message and phone number on the Lock screen.

Get the Location of a Device

Request the location of a device when in Lost Mode.

Play the Lost Mode Sound

Play the Lost Mode sound on a device that’s in Lost Mode.

