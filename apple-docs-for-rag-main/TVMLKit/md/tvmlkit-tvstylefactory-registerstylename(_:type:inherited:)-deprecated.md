

- TVMLKit
- TVStyleFactory
-  registerStyleName(\_:type:inherited:) Deprecated

Type Method

# registerStyleName(\_:type:inherited:)

Creates a new style property of the indicated type.

tvOS 9.0–18.0Deprecated

``` source
class func registerStyleName(
    _ styleName: String,
    type: TVViewElementStyleType,
    inherited: Bool
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`styleName`  

The name used to identify the style.

`type`  

The element style type as specified by TVViewElementStyleType.

`inherited`  

Boolean indicating whether the style is able to be inherited by other styles.

## See Also

### Creating New Style Properties

enum TVViewElementStyleType

Describes the different style types for an element.

Deprecated

