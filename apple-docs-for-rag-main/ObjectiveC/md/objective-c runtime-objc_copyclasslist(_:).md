

- Objective-C Runtime
-  objc_copyClassList(\_:) 

Function

# objc_copyClassList(\_:)

Creates and returns a list of pointers to all registered class definitions.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_copyClassList(_ outCount: UnsafeMutablePointer?) -> AutoreleasingUnsafeMutablePointer?
```

## Parameters 

`outCount`  

An integer pointer used to store the number of classes returned by this function in the list. This parameter may be `nil`.

## Return Value

A `nil` terminated array of classes. You must free the array with `free()`.

## See Also

### Obtaining Class Definitions

func objc_getClassList(AutoreleasingUnsafeMutablePointer&lt;AnyClass>?, Int32) -> Int32

Obtains the list of registered class definitions.

func objc_lookUpClass(UnsafePointer&lt;CChar>) -> AnyClass?

Returns the class definition of a specified class.

func objc_getClass(UnsafePointer&lt;CChar>) -> Any!

Returns the class definition of a specified class.

func objc_getRequiredClass(UnsafePointer&lt;CChar>) -> AnyClass

Returns the class definition of a specified class.

func objc_getMetaClass(UnsafePointer&lt;CChar>) -> Any!

Returns the metaclass definition of a specified class.

