

- App Clips
-  APActivationPayloadError 

Structure

# APActivationPayloadError

An error that an App Clip activation payload returns.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct APActivationPayloadError
```

## Topics

### Getting Information About the Error

static var errorDomain: String

### Error Codes

static var doesNotMatch: APActivationPayloadError.Code

The provided URL doesn’t match the invocation URL you registered for the App Clip.

static var disallowed: APActivationPayloadError.Code

The user denied location access, or the source of the App Clip invocation wasn’t an NFC tag or visual code.

enum Code

Error codes that an App Clip activation payload returns.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error Information

let APActivationPayloadErrorDomain: String

A string that identifies the activation payload’s error domain.

enum Code

Error codes that an App Clip activation payload returns.

