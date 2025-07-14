

- Device Management
-  Enable Declarative Management 

Web Service Endpoint

# Enable Declarative Management

Enable your server to support declarative management or trigger a declarative management synchronization operation on the device.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#DeclarativeManagementCommand
```

## HTTP Body

DeclarativeManagementCommand

The command to issue declarations to a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

DeclarativeManagementResponse

`OK`

A response from the device after it processes the command to issue declarations to a device.

Content-Type: application/xml

## Discussion

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | \-                                     |

### Example Request and Response

- Request
- Response

```

    Command

        CommandUUID
        0001_DeclarativeManagement
        Command

            RequestType
            DeclarativeManagement
            Data

            eyJTeW5jVG9rZW5zIjogeyJUaW1lc3RhbXAiOiAiMjAyMS0wNi0wMlQwMToy
            ODowMFoiLCAiRGVjbGFyYXRpb25zVG9rZW4iOiAiYjY1NDQwMjdhMzE1Y2Qw
            MDg1ZDRjZjA4MTc0NjI0YzJkMTQyNDQ0ODA0MzBhODdiMTc2YTI3MjdlNzM2
            NjEzOCJ9fQ==

```

```

    CommandUUID
    0001_DeclarativeManagement
    EnrollmentID
    8DB29EAB-A5BB-4B60-8DDA-F75517766FAC
    Status
    Acknowledged

```

## Topics

### Command and Response

object DeclarativeManagementCommand

The command to issue declarations to a device.

object DeclarativeManagementResponse

A response from the device after it processes the command to issue declarations to a device.

