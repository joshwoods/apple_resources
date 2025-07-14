

- WebKit
- WKContentWorld
-  name 

Instance Property

# name

The name of a custom content world.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var name: String? { get }
```

## Discussion

This property contains a valid string only for content worlds you retrieve using the world(name:) function. The value of this property is `nil` for the content worlds in the defaultClient and page properties.

## See Also

### Retrieving a Custom Content World

class func world(name: String) -> WKContentWorld

Returns the custom content world with the specified name.

