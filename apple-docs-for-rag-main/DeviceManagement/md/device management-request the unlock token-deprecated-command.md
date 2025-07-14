

- Device Management
-  Request the Unlock Token Deprecated

Web Service Endpoint

# Request the Unlock Token

Request an unlock token from a device.

iOS 5.0–6.1.6DeprecatediPadOS 5.0–6.1.6DeprecatedDevice Assignment ServicesVPP License Management

Deprecated

Apple has deprecated this command. The MDM server receives `UnlockToken`s from the TokenUpdateRequest.

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RequestUnlockTokenCommand
```

## HTTP Body

RequestUnlockTokenCommand

The command to request an unlock token from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RequestUnlockTokenResponse

`OK`

A response from the device after it processes the request for an unlock token.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                             |
|----------------------------|-----------------------------|
| Device Channel             | iOS                         |
| User Channel               | \-                          |
| Requires Supervision       | iOS                         |
| Allowed in User Enrollment | \-                          |
| Required Access Right      | AllowPasscodeRemovalAndLock |

## Topics

### Command and Response

object RequestUnlockTokenCommand

The command to request an unlock token from a device.

object RequestUnlockTokenResponse

A response from the device after it processes a request for an unlock token.

