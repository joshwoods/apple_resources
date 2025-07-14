

- UIKit
- UIApplication
- UIApplication.CategoryDefaultError
-  UIApplication.CategoryDefaultError.Code 

Enumeration

# UIApplication.CategoryDefaultError.Code

An enumeration of reasons an error happens when the system discovers whether your app is the default in a category.

iOS 18.2+iPadOS 18.2+

``` source
enum Code
```

## Topics

### Error codes

case rateLimited

The system didn’t determine if your app is the default in a category because the app made the request too many times.

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

### Getting information about the error

static let retryAvailableDateErrorKey: String

A dictionary key, with a value that’s a date when a result is next available.

static let statusLastProvidedDateErrorKey: String

A dictionary key, with a value that’s the date your app last received a successful result.

