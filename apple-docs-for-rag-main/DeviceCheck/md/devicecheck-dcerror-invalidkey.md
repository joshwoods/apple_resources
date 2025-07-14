

- DeviceCheck
- DCError
-  invalidKey 

Type Property

# invalidKey

An error caused by a failed attempt to use the App Attest key.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
static var invalidKey: DCError.Code { get }
```

## Discussion

You receive this error if something goes wrong with generating, retrieving, or using an App Attest cryptographic key, when:

- You call attestKey(_:clientDataHash:completionHandler:) for a key that’s already been attested.

- You call generateAssertion(_:clientDataHash:completionHandler:) with an unattested key.

- The App Attest service rejects the key.

## See Also

### Errors

static var featureUnsupported: DCError.Code

DeviceCheck is not available on this device.

static var invalidInput: DCError.Code

An error code that indicates when your app provides data that isn’t formatted correctly.

static var serverUnavailable: DCError.Code

An error that indicates a failed attempt to contact the App Attest service during an attestation.

static var unknownSystemFailure: DCError.Code

A failure has occurred, such as the failure to generate a token.

enum Code

DeviceCheck error codes.

