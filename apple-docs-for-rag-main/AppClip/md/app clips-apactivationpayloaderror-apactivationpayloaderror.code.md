

- App Clips
- APActivationPayloadError
-  APActivationPayloadError.Code 

Enumeration

# APActivationPayloadError.Code

Error codes that an App Clip activation payload returns.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum Code
```

## Topics

### Enumeration Values

case doesNotMatch

The provided URL doesn’t match the registered App Clip URL.

case disallowed

The user denied location access, or the source of the App Clip invocation wasn’t from an NFC tag or visual code.

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

### Error Information

let APActivationPayloadErrorDomain: String

A string that identifies the activation payload’s error domain.

struct APActivationPayloadError

An error that an App Clip activation payload returns.

