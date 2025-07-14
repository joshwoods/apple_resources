

- Device Management
-  Declarations 

Device Management Profile

# Declarations

The payload to apply a set of declaration to the device through the Settings app.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object Declarations
```

## Properties

`Declarations`

`[data]`

 (Required) 

The set of declarations to apply. The items in this array are Base64-encoded data representations of the declaration JSON data.

## Discussion

Specify `com.apple.declarations` as the payload type.

Note

Install this profile manually, not through an MDM server, which enables manual installations of declarations when an MDM enrollment isn’t present.

### Profile Availability

|                            |                           |
|----------------------------|---------------------------|
| Device Channel             | iOS, macOS, tvOS, watchOS |
| User Channel               | \-                        |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS |
| Requires Supervision       | \-                        |
| Requires User Approved MDM | \-                        |
| Allowed in User Enrollment | \-                        |
| Allow Multiple Payloads    | iOS, macOS, tvOS, watchOS |

### Profile Example

```

    PayloadContent

            Declarations

                ewogICJUeXBlIjogImNvbS5hcHBsZS5hY3RpdmF0aW9u
                LnNpbXBsZSIsCiAgIklkZW50aWZpZXIiOiAiMzJGOUVF
                RkMtQzM5QS00QjI5LUJCRjgtNUM5Q0RBQTIyMDU3IiwK
                ICAiU2VydmVyVG9rZW4iOiAiODhFMjUzQjctNzYyNC00
                QUNGLTg1NTEtMzA4RDgyMUM0Njg0IiwKICAiUGF5bG9h
                ZCI6IHsKICAgICJTdGFuZGFyZENvbmZpZ3VyYXRpb25z
                IjogWwogICAgICAiMDdBMUUxNDgtMkM2Ri00Mzk0LTk4
                RTctNzRFMjA1RTAxQjIwIgogICAgXQogIH0KfQo=

                ewogICJUeXBlIjogImNvbS5hcHBsZS5jb25maWd1cmF0
                aW9uLm1hbmFnZW1lbnQudGVzdCIsCiAgIklkZW50aWZp
                ZXIiOiAiMDdBMUUxNDgtMkM2Ri00Mzk0LTk4RTctNzRF
                MjA1RTAxQjIwIiwKICAiU2VydmVyVG9rZW4iOiAiRUIy
                N0U5RjctRkZGQi00MUJFLTk4MEMtRThBNUZCODAxMzky
                IiwKICAiUGF5bG9hZCI6IHsKICAgICJFY2hvIjogIkVj
                aG8gdGhpcyBtZXNzYWdlIiwKICAgICJSZXR1cm5TdGF0
                dXMiOiAiSW5zdGFsbGVkIgogIH0KfQo=

            PayloadDescription
            Configures a set of declarations
            PayloadDisplayName
            Declarations profile
            PayloadIdentifier
            com.apple.declarations.2a3f8721-352d-48c0-a83d-737dc64589ad
            PayloadType
            com.apple.declarations
            PayloadUUID
            5edd1fa1-31ce-43ee-a6dc-8e0bed5e9c20
            PayloadVersion
            1

    PayloadDisplayName
    Test Declaration
    PayloadIdentifier
    declarations-5959abc0-1135-4d22-8ff0-a170bcceb3c8
    PayloadRemovalDisallowed

    PayloadType
    Configuration
    PayloadUUID
    5959abc0-1135-4d22-8ff0-a170bcceb3c8
    PayloadVersion
    1

```

## See Also

### System Configuration

object EnergySaver

The payload you use to configure energy-saver settings.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

