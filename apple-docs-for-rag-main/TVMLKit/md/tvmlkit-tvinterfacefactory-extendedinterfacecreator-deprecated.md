

- TVMLKit
- TVInterfaceFactory
-  extendedInterfaceCreator Deprecated

Instance Property

# extendedInterfaceCreator

The interface that is being extended.

tvOS 9.0–18.0Deprecated

``` source
var extendedInterfaceCreator: (any TVInterfaceCreating)? { get set }
```

Deprecated

Please use SwiftUI or UIKit

## Mentioned in 

Creating TVML Elements

## Discussion

An app can extend or override framework implementation by setting the extendedInterfaceCreator property. An app must provide its own methods to handle custom registered elements.

## See Also

### Extending an Interface

class func shared() -> Self

Returns the singleton instance of the interface factory.

Deprecated

