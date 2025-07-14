

- Objective-C Runtime
-  objc_copyImageNames(\_:) 

Function

# objc_copyImageNames(\_:)

Returns the names of all the loaded Objective-C frameworks and dynamic libraries.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_copyImageNames(_ outCount: UnsafeMutablePointer?) -> UnsafeMutablePointer>
```

## Parameters 

`outCount`  

The number of names in the returned array.

## Return Value

An array of C strings representing the names of all the loaded Objective-C frameworks and dynamic libraries.

## See Also

### Working with Libraries

func class_getImageName(AnyClass?) -> UnsafePointer&lt;CChar>?

Returns the name of the dynamic library a class originated from.

func objc_copyClassNamesForImage(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>?

Returns the names of all the classes within a specified library or framework.

