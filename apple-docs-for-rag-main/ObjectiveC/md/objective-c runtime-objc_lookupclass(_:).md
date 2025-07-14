

- Objective-C Runtime
-  objc_lookUpClass(\_:) 

Function

# objc_lookUpClass(\_:)

Returns the class definition of a specified class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_lookUpClass(_ name: UnsafePointer) -> AnyClass?
```

## Parameters 

`name`  

The name of the class to look up.

## Return Value

The Class object for the named class, or `nil` if the class is not registered with the Objective-C runtime.

## Discussion

The implementation of this function is identical to the implementation of the objc_getClass(_:) function.

## See Also

### Obtaining Class Definitions

func objc_getClassList(AutoreleasingUnsafeMutablePointer&lt;AnyClass>?, Int32) -> Int32

Obtains the list of registered class definitions.

func objc_copyClassList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;AnyClass>?

Creates and returns a list of pointers to all registered class definitions.

func objc_getClass(UnsafePointer&lt;CChar>) -> Any!

Returns the class definition of a specified class.

func objc_getRequiredClass(UnsafePointer&lt;CChar>) -> AnyClass

Returns the class definition of a specified class.

func objc_getMetaClass(UnsafePointer&lt;CChar>) -> Any!

Returns the metaclass definition of a specified class.

