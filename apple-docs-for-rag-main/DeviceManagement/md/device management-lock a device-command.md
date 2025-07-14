

- Device Management
-  Lock a Device 

Web Service Endpoint

# Lock a Device

Remotely and immediately lock a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeviceLockCommand
```

## HTTP Body

DeviceLockCommand

The command to lock a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeviceLockResponse

`OK`

A response from the device after it processes the command to lock.

Content-Type: application/xml

## Discussion

You can display a message and phone number on the Lock screen if the user has set a passcode for the device, it isn’t a shared iPad device, and it isn’t in Lost Mode. In macOS, this command uses the Find My framework to lock a device, and fails if there’s no recovery partition on the device.

Warning

Sending this command to a Mac with Apple silicon running a version of macOS before 11.5 deactivates the Mac. To reactivate that Mac, it needs a network connection and authentication by a local administrator with Secure Token enabled.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                  |
|----------------------------|----------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, watchOS |
| User Channel               | \-                               |
| Requires Supervision       | \-                               |
| Allowed in User Enrollment | iOS                              |
| Required Access Right      | AllowPasscodeRemovalAndLock      |

### Example Request and Response

- Request
- Response

```

    Command

        Message
        Lock Message
        PhoneNumber
        408-555-5555
        RequestType
        DeviceLock

    CommandUUID
    0001_DeviceLock

```

```

    CommandUUID
    0001_DeviceLock
    MessageResult
    Success
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object DeviceLockCommand

The command to lock a device.

object DeviceLockResponse

A response from the device after it processes the command to lock.

## See Also

### Device State

Erase a Device

Remotely and immediately erase a device.

Restart a Device

Remotely and immediately restart a device.

Shut Down a Device

Remotely and immediately shut down a device.

