

- Device Management
-  List the Installed Restrictions 

Web Service Endpoint

# List the Installed Restrictions

Get a list of restrictions on the device.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RestrictionsCommand
```

## HTTP Body

RestrictionsCommand

The command to get a list of restrictions on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RestrictionsResponse

`OK`

A response from the device after it processes the command to get a list of restrictions.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                                 |
|----------------------------|---------------------------------|
| Device Channel             | iOS, Shared iPad, tvOS, watchOS |
| User Channel               | Shared iPad                     |
| Requires Supervision       | \-                              |
| Allowed in User Enrollment | \-                              |
| Required Access Right      | AllowQueryRestrictions          |

### Example Request and Response

- Request
- Response

```

    Command

        ProfileRestrictions

        RequestType
        Restrictions

    CommandUUID
    0001_Restrictions

```

```

    CommandUUID
    0001_Restrictions
    GlobalRestrictions

        restrictedBool

            allowCamera

                value

    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RestrictionsCommand

The command to get a list of restrictions on a device.

object RestrictionsResponse

A response from the device after it processes the command to get a list of restrictions.

## See Also

### Device Details

List the Installed Apps

Get a list of the installed apps on a device.

Get Device Information

Get detailed information about a device.

Release Device from Await Configuration

Inform the device that it can allow the user to continue in Setup Assistant.

User Configured Command

Informs the device that it can continue past Setup Assistant and finish login.

