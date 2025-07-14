

- UIKit
- UIDocument
-  UIDocument.CreationIntent 

Structure

# UIDocument.CreationIntent

An app intent that creates new documents for your app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct CreationIntent
```

## Mentioned in 

Customizing a document-based app’s launch experience

## Overview

UIKit provides a default intent. You can extend this structure to provide additional intents for your app.

```
// Extend the creation intent enumeration to add custom options for document creation.
extension UIDocument.CreationIntent {
    static let template = UIDocument.CreationIntent("template")
}
```

For more information, see Customizing a document-based app’s launch experience.

## Topics

### Accessing creation intents

static let `default`: UIDocument.CreationIntent

The default document creation intent.

### Creating new intents

init(String)

Create a new document creation intent using the provided string.

init(rawValue: String)

Create a new document creation intent using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

