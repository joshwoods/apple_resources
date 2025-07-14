

- Objective-C Runtime
-  objc_getMetaClass(\_:) 

Function

# objc_getMetaClass(\_:)

Returns the metaclass definition of a specified class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_getMetaClass(_ name: UnsafePointer) -> Any!
```

## Parameters 

`name`  

The name of the class to look up.

## Return Value

The `Class` object for the metaclass of the named class, or `nil` if the class is not registered with the Objective-C runtime.

## Discussion

If the definition for the named class is not registered, this function calls the class handler callback and then checks a second time to see if the class is registered. However, every class definition must have a valid metaclass definition, and so the metaclass definition is always returned, whether it’s valid or not.

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

func objc_getRequiredClass(UnsafePointer&lt;CChar>) -> AnyClass

Returns the class definition of a specified class.

