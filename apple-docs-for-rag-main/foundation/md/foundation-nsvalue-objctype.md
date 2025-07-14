

- Foundation
- NSValue
-  objCType 

Instance Property

# objCType

A C string containing the Objective-C type of the data contained in the value object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var objCType: UnsafePointer { get }
```

## Discussion

This property provides the same string produced by the `@encode()` compiler directive.

## See Also

### Working with Raw Values

init(bytes: UnsafeRawPointer, objCType: UnsafePointer&lt;CChar>)

Initializes a value object to contain the specified value, interpreted with the specified Objective-C type.

init(UnsafeRawPointer, withObjCType: UnsafePointer&lt;CChar>)

Creates a value object containing the specified value, interpreted with the specified Objective-C type.

func getValue(UnsafeMutableRawPointer)

Copies the value into the specified buffer.

