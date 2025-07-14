

- TVMLKit
-  TVElementFactory Deprecated

Class

# TVElementFactory

An object used to register new elements to extend the Apple TV Markup Language (TVML).

tvOS 9.0–18.0Deprecated

``` source
class TVElementFactory
```

Deprecated

Please use SwiftUI or UIKit

## Overview

You must register new elements before initializing a TVApplicationController object.

## Topics

### Registering New Elements

class func registerViewElementClass(AnyClass, elementName: String)

Registers a view element for the specified element name.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Custom Elements

class TVImageElement

A representation of a read-only DOM node containing the attributes that describe an image element.

Deprecated

class TVTextElement

The textual content for the DOM element.

Deprecated

Creating TVML Elements

Avoid rewriting complex and often used elements by creating a simplified custom element.

