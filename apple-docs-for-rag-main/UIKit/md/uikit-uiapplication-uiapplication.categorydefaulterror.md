

- UIKit
- UIApplication
-  UIApplication.CategoryDefaultError 

Structure

# UIApplication.CategoryDefaultError

Errors that can happen when the system checks if your app is the default app in a category.

iOS 18.2+iPadOS 18.2+

``` source
struct CategoryDefaultError
```

## Topics

### Getting information about the error

enum Code

An enumeration of reasons an error happens when the system discovers whether your app is the default in a category.

static let retryAvailableDateErrorKey: String

A dictionary key, with a value that’s a date when a result is next available.

static let statusLastProvidedDateErrorKey: String

A dictionary key, with a value that’s the date your app last received a successful result.

### Errors when discovering if an app is the default in a category

static var errorDomain: String

A string that indicates that an error happened when the system attempted to determine if your app is the default in a category.

static var rateLimited: UIApplication.CategoryDefaultError.Code

An error code that indicates your app requested its status too frequently.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Discovering if your app is the default app in a category

func isDefault(UIApplication.Category) throws -> Bool

Reports whether this app is the person’s default app in the given category.

enum Category

Constants that describe the types of apps in the system.

