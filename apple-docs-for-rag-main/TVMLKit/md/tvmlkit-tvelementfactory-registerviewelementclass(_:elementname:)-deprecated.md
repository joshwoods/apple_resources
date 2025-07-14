

- TVMLKit
- TVElementFactory
-  registerViewElementClass(\_:elementName:) Deprecated

Type Method

# registerViewElementClass(\_:elementName:)

Registers a view element for the specified element name.

tvOS 9.0–18.0Deprecated

``` source
class func registerViewElementClass(
    _ elementClass: AnyClass,
    elementName: String
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`elementClass`  

The class of the element.

`elementName`  

The element name used when referencing this element within TVML.

## Mentioned in 

Creating TVML Elements

## Discussion

The TVViewElement class represents a read-only DOM node along with its attributes and aggregated style. This model object is traversed by the interface factory to construct views and view controllers, and to render templates. You must call this method for each element you register.

