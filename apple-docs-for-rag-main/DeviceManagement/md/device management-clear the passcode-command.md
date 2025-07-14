

- Device Management
-  Clear the Passcode 

Web Service Endpoint

# Clear the Passcode

Remove the passcode from a device.

iOS 4.0+iPadOS 4.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ClearPasscodeCommand
```

## HTTP Body

ClearPasscodeCommand

The command to clear the passcode on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ClearPasscodeResponse

`OK`

A response from the device after it processes the command to remove the passcode from a device.

Content-Type: application/xml

## Discussion

Clearing the passcode in iOS 16 no longer adds the passcode to the history of passcodes. Therefore, the user can reuse the cleared passcode even when the `Passcode` payload has the `pinHistory` key set.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | iOS, watchOS                |
| User Channel               | \-                          |
| Requires Supervision       | \-                          |
| Allowed in User Enrollment | \-                          |
| Required Access Right      | AllowPasscodeRemovalAndLock |

### Example Request and Response

- Request
- Response

```

    Command

        RequestType
        ClearPasscode
        UnlockToken

        REFUQQAABPRWRVJTAAAABAAAAAVUWVBFAAAABAAAAAJVVUlEAAAAEGHX7XgO5UNZsRiL
        9Kq3hSdITUNLAAAAKLUR5mc5hBzI4bEsbWacE/gmhdJS6rl3978V3DY9ylBbEBGgJ/fA
        Ac9XUkFQAAAABAAAAAFTQUxUAAAAFIHju7P8BPFTz0JA8MDo+PsvcAAmSVRFUgAAAAQA
        AEEaVVVJRAAAABC70Oy5TtZCGocX/i7orO/pQ0xBUwAAAAQAAAABV1JBUAAAAAQAAAAD
        S1RZUAAAAAQAAAAAV1BLWQAAACjH8wUEvSkfgrEPSSQUazAz1eCuTXET3CkqgkNQZkjS
        jZEHtWmXpC4IVVVJRAAAABBW4TUxIb1L7aNAmbmGkxiIQ0xBUwAAAAQAAAACV1JBUAAA
        AAQAAAADS1RZUAAAAAQAAAABV1BLWQAAAChaDERvmDXtk9mikMCT30uDQ4XwrT9ifdmf
        3Hjz/6atBPq/1uNpm5TtUEJLWQAAACCypmyEJV4x4wV6CKfZFEmkYHf8kOXh5ONM1A6B
        R26KM1VVSUQAAAAQH5Ol3/mLSM2dLvFxGTlf5kNMQVMAAAAEAAAAA1dSQVAAAAAEAAAA
        A0tUWVAAAAAEAAAAAFdQS1kAAAAoxNNjRWfqvgqXMVyiqDH2LXJdpafgsm+8ovRQuzL4
        tp3Bs5y25bmRelVVSUQAAAAQB7drprzaR5aePknqFUjyWENMQVMAAAAEAAAABVdSQVAA
        AAAEAAAAA0tUWVAAAAAEAAAAAFdQS1kAAAAoMCe2S7psda5AHw99a+DKV8m0hR6aKUKP
        VG5oURKAJZSXJKYRRO2xKlVVSUQAAAAQMpEnWAWOS0qnOwWRdtSAlUNMQVMAAAAEAAAA
        BldSQVAAAAAEAAAAA0tUWVAAAAAEAAAAAFdQS1kAAAAoyhn4O/EIo5Q1NLt0/wL1UZGA
        EqTE45DEcNstAQZLk+1U/FSKOWtqrlVVSUQAAAAQFuJUehe6TC+3TImCkemk6kNMQVMA
        AAAEAAAAB1dSQVAAAAAEAAAAA0tUWVAAAAAEAAAAAFdQS1kAAAAoMcyPJI8vNBh7j6je
        VPu3zgDYTXAuoo68jqZU4kCubSGyRvIpa/O4n1VVSUQAAAAQF2v1dlxfRMqYs7swzn9s
        nENMQVMAAAAEAAAACFdSQVAAAAAEAAAAA0tUWVAAAAAEAAAAAFdQS1kAAAAoSx2pMsvH
        K2HNg9IIbrVEzX7T3Rw0vLEmwMJ3ignooj+3GMHeaJ0aplVVSUQAAAAQ8Qif3NCoTjiK
        WRjgOIHG6ENMQVMAAAAEAAAACVdSQVAAAAAEAAAAA0tUWVAAAAAEAAAAAFdQS1kAAAAo
        n2icCfaIRPbE7mzGqO7rOnuPhgUbYkcpAqf6RnAXljcpSxZqBiJtGlVVSUQAAAAQt9a3
        ThB7SwaGw50i9Hhfu0NMQVMAAAAEAAAACldSQVAAAAAEAAAAA0tUWVAAAAAEAAAAAFdQ
        S1kAAAAoEW1/yC+YYXLVzyRxZwghOADACnWvOnHdBPhJ/z7VEkyHcObDPI9w41VVSUQA
        AAAQ4vImTUp5S7qmyMDZ82nM70NMQVMAAAAEAAAAC1dSQVAAAAAEAAAAA0tUWVAAAAAE
        AAAAAFdQS1kAAAAo8vkvhYNP7rTLdfXRifh+dcTIbj3EEJKyYXeCL9J9trYAo7B5mV5u
        41NJR04AAAAUtFVbS3MM33WvBsEis1imzvs069A=

    CommandUUID
    0001_ClearPasscode

```

```

    CommandUUID
    0001_ClearPasscode
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ClearPasscodeCommand

The command to clear the passcode on a device.

object ClearPasscodeResponse

A response from the device after it processes the command to remove the passcode from a device.

## See Also

### Passwords

Clear the Restrictions Password

Clear the restrictions password and the restrictions on a device.

Unlock a User Account

Unlock a user account that the system locked because of too many failed password attempts.

Set the Local Administrator Password

Update the local administrator account password.

Set the Firmware Password

Change or clear the firmware password on a device.

Verify the Firmware Password

Verify the firmware password on a device.

