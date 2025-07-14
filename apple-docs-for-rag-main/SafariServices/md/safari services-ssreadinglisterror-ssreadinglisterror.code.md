

- Safari Services
- SSReadingListError
-  SSReadingListError.Code 

Enumeration

# SSReadingListError.Code

Messages that describe a Safari Reading List error.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+visionOS 1.0+

**Mac Catalyst**

``` source
enum SSReadingListErrorCode
```

**iOS, iPadOS, visionOS**

``` source
enum Code
```

## Topics

### Constants

case urlSchemeNotAllowed

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

### Safari Reading List

class SSReadingList

An object for adding items to a user’s Safari Reading List.

let SSReadingListErrorDomain: String

The domain for Safari Reading List errors.

struct SSReadingListError

A Safari Reading List error.

