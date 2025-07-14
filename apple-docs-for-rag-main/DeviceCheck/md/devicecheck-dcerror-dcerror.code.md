

- DeviceCheck
- DCError
-  DCError.Code 

Enumeration

# DCError.Code

DeviceCheck error codes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+tvOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Error codes

case featureUnsupported

DeviceCheck is unavailable on this device.

case invalidInput

An error code that indicates when your app provides data that isn’t formatted correctly.

case invalidKey

An error caused by a failed attempt to use the App Attest key.

case serverUnavailable

An error that indicates a failed attempt to contact the App Attest service during an attestation.

case unknownSystemFailure

A failure has occurred, such as the failure to generate a token.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct DCError

A type that indicates when DeviceCheck encounters an error.

let DCErrorDomain: String

The error domain for errors associated with DeviceCheck APIs.

