

- Objective-C Runtime
-  objc_getRequiredClass(\_:) 

Function

# objc_getRequiredClass(\_:)

Returns the class definition of a specified class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_getRequiredClass(_ name: UnsafePointer) -> AnyClass
```

## Parameters 

`name`  

The name of the class to look up.

## Return Value

The Class object for the named class.

## Discussion

This function is the same as objc_getClass(_:), but kills the process if the class is not found.

This function is used by ZeroLink, where failing to find a class would be a compile-time link error without ZeroLink.

## See Also

### Obtaining Class Definitions

func objc_getClassList(AutoreleasingUnsafeMutablePointer&lt;AnyClass>?, Int32) -> Int32

Obtains the list of registered class definitions.

func objc_copyClassList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;AnyClass>?

Creates and returns a list of pointers to all registered class definitions.

func objc_lookUpClass(UnsafePointer&lt;CChar>) -> AnyClass?

Returns the class definition of a specified class.

func objc_getClass(UnsafePointer&lt;CChar>) -> Any!

Returns the class definition of a specified class.

func objc_getMetaClass(UnsafePointer&lt;CChar>) -> Any!

Returns the metaclass definition of a specified class.

