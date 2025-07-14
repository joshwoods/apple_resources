

- Device Management
- GetTokenRequest
-  GetTokenRequest.TokenParameters 

Device Management Command

# GetTokenRequest.TokenParameters

Parameters that the system uses to generate the token.

iOS 17.0+iPadOS 17.0+macOS 14.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object GetTokenRequest.TokenParameters
```

## Properties

`PhoneUDID`

`string`

The identifier of the phone paired to the watch. Required by the `com.apple.watch.pairing` service type.

`SecurityToken`

`string`

A security token to generate the server token. Required by the `com.apple.watch.pairing` service type.

`WatchUDID`

`string`

The identifier of the watch paired to the phone. Required by the `com.apple.watch.pairing` service type.

