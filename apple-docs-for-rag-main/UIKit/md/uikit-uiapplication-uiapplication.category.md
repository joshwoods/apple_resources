

- UIKit
- UIApplication
-  UIApplication.Category 

Enumeration

# UIApplication.Category

Constants that describe the types of apps in the system.

iOS 18.2+iPadOS 18.2+

``` source
enum Category
```

## Overview

Use the values in this enumeration with isDefault(_:) (or, in Objective-C, defaultStatusForCategory:error:) to find if your app is the person’s default for a category.

## Topics

### Application categories

case webBrowser

The app is a web browser.

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

### Discovering if your app is the default app in a category

func isDefault(UIApplication.Category) throws -> Bool

Reports whether this app is the person’s default app in the given category.

struct CategoryDefaultError

Errors that can happen when the system checks if your app is the default app in a category.

