

- Device Management
-  Enable Lost Mode 

Web Service Endpoint

# Enable Lost Mode

Enable Lost Mode on a device, which provides a message and phone number on the Lock screen.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#EnableLostModeCommand
```

## HTTP Body

EnableLostModeCommand

The command to enable Lost Mode.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

EnableLostModeResponse

`OK`

A response from the device after it processes the command to enable Lost Mode.

Content-Type: application/xml

## Discussion

While in Lost Mode, a device responds to invalid commands with error code `12078`.

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

        Footnote
        Return to Acme, Inc.
        Message
        Lock Message
        PhoneNumber
        408-555-555
        RequestType
        EnableLostMode

    CommandUUID
    0001_EnableLostMode

```

```

    CommandUUID
    0001_EnableLostMode
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object EnableLostModeCommand

The command to enable Lost Mode.

object EnableLostModeResponse

A response from the device after it processes the command to enable Lost Mode.

## See Also

### Lost Device

Get the Location of a Device

Request the location of a device when in Lost Mode.

Play the Lost Mode Sound

Play the Lost Mode sound on a device that’s in Lost Mode.

Disable Lost Mode

Take the device out of Lost Mode.

