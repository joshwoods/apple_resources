

- ClassKit
-  CLSErrorUserInfoKey 

Structure

# CLSErrorUserInfoKey

Keys that appear in the user info dictionary in errors that ClassKit creates.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
struct CLSErrorUserInfoKey
```

## Topics

### Keys

static let objectKey: CLSErrorUserInfoKey

A key whose value is the object that caused the error.

static let successfulObjectsKey: CLSErrorUserInfoKey

static let underlyingErrorsKey: CLSErrorUserInfoKey

A key whose value is the array of errors that contributed to this error.

### Initializers

init(String)

Initializes the key.

init(rawValue: String)

Initializes the key with a value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct CLSError

Errors issued by ClassKit.

let CLSErrorCodeDomain: String

The error domain that ClassKit uses when issuing errors.

enum Code

Error codes that ClassKit issues.

