

- Objective-C Runtime
-  class_getImageName(\_:) 

Function

# class_getImageName(\_:)

Returns the name of the dynamic library a class originated from.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func class_getImageName(_ cls: AnyClass?) -> UnsafePointer?
```

## Parameters 

`cls`  

The class you are inquiring about.

## Return Value

A C string representing the name of the library containing the `cls` class.

## See Also

### Working with Libraries

func objc_copyImageNames(UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>

Returns the names of all the loaded Objective-C frameworks and dynamic libraries.

func objc_copyClassNamesForImage(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>>?

Returns the names of all the classes within a specified library or framework.

