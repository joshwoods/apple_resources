

- Objective-C Runtime
-  objc_copyClassNamesForImage(\_:\_:) 

Function

# objc_copyClassNamesForImage(\_:\_:)

Returns the names of all the classes within a specified library or framework.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_copyClassNamesForImage(
    _ image: UnsafePointer,
    _ outCount: UnsafeMutablePointer?
) -> UnsafeMutablePointer>?
```

## Parameters 

`image`  

The library or framework you are inquiring about.

`outCount`  

The number of class names in the returned array.

## Return Value

An array of C strings representing all of the class names within the specified library or framework.

## See Also

### Working with Libraries

func objc_copyImageNames(UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>

Returns the names of all the loaded Objective-C frameworks and dynamic libraries.

func class_getImageName(AnyClass?) -> UnsafePointer&lt;CChar>?

Returns the name of the dynamic library a class originated from.

