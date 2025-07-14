

- Device Management
-  Play the Lost Mode Sound 

Web Service Endpoint

# Play the Lost Mode Sound

Play the Lost Mode sound on a device that’s in Lost Mode.

iOS 10.3+iPadOS 10.3+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#PlayLostModeSoundCommand
```

## HTTP Body

PlayLostModeSoundCommand

The command to play the Lost Mode sound.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

PlayLostModeSoundResponse

`OK`

A response from the device after it processes the command to play the Lost Mode sound.

Content-Type: application/xml

## Discussion

A device responds with error code `12067` if it isn’t in Lost Mode. While in Lost Mode, a device responds to invalid commands with error code `12078`.

The sound plays until the server disables Lost Mode or the user disables the sound on the device.

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
        PlayLostModeSound

    CommandUUID
    0001_PlayLostModeSound

```

```

    CommandUUID
    0001_PlayLostModeSound
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object PlayLostModeSoundCommand

The command to play the Lost Mode sound.

object PlayLostModeSoundResponse

A response from the device in Lost Mode after it processes the command to play the Lost Mode sound.

## See Also

### Lost Device

Enable Lost Mode

Enable Lost Mode on a device, which provides a message and phone number on the Lock screen.

Get the Location of a Device

Request the location of a device when in Lost Mode.

Disable Lost Mode

Take the device out of Lost Mode.

