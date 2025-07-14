

- Core Graphics
- CGLayer
-  typeID 

Type Property

# typeID

Returns the unique type identifier used for CGLayer objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class var typeID: CFTypeID { get }
```

## Discussion

A type identifier is an integer that identifies the opaque type to which a Core Foundation object belongs. You use type IDs in various contexts, such as when you are operating on heterogeneous collections.

