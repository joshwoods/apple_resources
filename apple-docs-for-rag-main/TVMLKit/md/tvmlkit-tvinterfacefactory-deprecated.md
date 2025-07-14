

- TVMLKit
-  TVInterfaceFactory Deprecated

Class

# TVInterfaceFactory

A factory for the creation of views and view controllers.

tvOS 9.0–18.0Deprecated

``` source
class TVInterfaceFactory
```

Deprecated

Please use SwiftUI or UIKit

## Overview

The app can extend or override the framework implementation by setting extendedInterfaceCreator.

## Topics

### Extending an Interface

var extendedInterfaceCreator: (any TVInterfaceCreating)?

The interface that is being extended.

class func shared() -> Self

Returns the singleton instance of the interface factory.

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
- TVInterfaceCreating

## See Also

### Views and View Controllers

class TVViewElement

A representation of a read-only DOM node.

Deprecated

protocol TVInterfaceCreating

A protocol that defines methods used to create views and view controllers.

Deprecated

class TVBrowserViewController

A view controller that presents content in a browsable, full-screen format.

class TVDocumentViewController

A view controller that represents a TVMLKit document.

Deprecated

