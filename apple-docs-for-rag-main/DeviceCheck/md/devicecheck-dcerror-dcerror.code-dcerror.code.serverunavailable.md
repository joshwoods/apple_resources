

- DeviceCheck
- DCError
- DCError.Code
-  DCError.Code.serverUnavailable 

Case

# DCError.Code.serverUnavailable

An error that indicates a failed attempt to contact the App Attest service during an attestation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
case serverUnavailable
```

## Discussion

You receive this error when you call attestKey(_:clientDataHash:completionHandler:) and the framework isn’t able to complete the attestation. If you receive this error, try the attestation again later using the same key and the same value for the `clientDataHash` parameter. Retrying with the same inputs helps to preserve the risk metric for a given device.

## See Also

### Error codes

case featureUnsupported

DeviceCheck is unavailable on this device.

case invalidInput

An error code that indicates when your app provides data that isn’t formatted correctly.

case invalidKey

An error caused by a failed attempt to use the App Attest key.

case unknownSystemFailure

A failure has occurred, such as the failure to generate a token.

