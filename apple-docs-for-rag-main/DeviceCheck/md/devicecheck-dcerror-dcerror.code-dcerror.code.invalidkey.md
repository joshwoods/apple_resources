

- DeviceCheck
- DCError
- DCError.Code
-  DCError.Code.invalidKey 

Case

# DCError.Code.invalidKey

An error caused by a failed attempt to use the App Attest key.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
case invalidKey
```

## Discussion

You receive this error if something goes wrong with generating, retrieving, or using an App Attest cryptographic key, when:

- You call attestKey(_:clientDataHash:completionHandler:) for a key that’s already been attested.

- You call generateAssertion(_:clientDataHash:completionHandler:) with an unattested key.

- The App Attest service rejects the key.

## See Also

### Error codes

case featureUnsupported

DeviceCheck is unavailable on this device.

case invalidInput

An error code that indicates when your app provides data that isn’t formatted correctly.

case serverUnavailable

An error that indicates a failed attempt to contact the App Attest service during an attestation.

case unknownSystemFailure

A failure has occurred, such as the failure to generate a token.

