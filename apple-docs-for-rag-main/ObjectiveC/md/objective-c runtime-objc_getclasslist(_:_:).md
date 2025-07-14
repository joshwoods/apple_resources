

- Objective-C Runtime
-  objc_getClassList(\_:\_:) 

Function

# objc_getClassList(\_:\_:)

Obtains the list of registered class definitions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_getClassList(
    _ buffer: AutoreleasingUnsafeMutablePointer?,
    _ bufferCount: Int32
) -> Int32
```

## Parameters 

`buffer`  

An array of `Class` values. On output, each `Class` value points to one class definition, up to either `bufferCount` or the total number of registered classes, whichever is less. You can pass `NULL` to obtain the total number of registered class definitions without actually retrieving any class definitions.

`bufferCount`  

An integer value. Pass the number of pointers for which you have allocated space in `buffer`. On return, this function fills in only this number of elements. If this number is less than the number of registered classes, this function returns an arbitrary subset of the registered classes.

## Return Value

An integer value indicating the total number of registered classes.

## Discussion

The Objective-C runtime library automatically registers all the classes defined in your source code. You can create class definitions at runtime and register them with the `objc_addClass` function.

The code listing below demonstrates how to use this function to retrieve all the class definitions that have been registered with the Objective-C runtime in the current process.

```
int numClasses;
Class * classes = NULL;

classes = NULL;
numClasses = objc_getClassList(NULL, 0);

if (numClasses > 0 )
{
    classes = malloc(sizeof(Class) * numClasses);
    numClasses = objc_getClassList(classes, numClasses);
    free(classes);
}
```

### Special Considerations

You can’t assume that class objects you get from this function are classes that inherit from NSObject, so you can’t safely call any methods on such classes without detecting that the method is implemented first.

## See Also

### Obtaining Class Definitions

func objc_copyClassList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;AnyClass>?

Creates and returns a list of pointers to all registered class definitions.

func objc_lookUpClass(UnsafePointer&lt;CChar>) -> AnyClass?

Returns the class definition of a specified class.

func objc_getClass(UnsafePointer&lt;CChar>) -> Any!

Returns the class definition of a specified class.

func objc_getRequiredClass(UnsafePointer&lt;CChar>) -> AnyClass

Returns the class definition of a specified class.

func objc_getMetaClass(UnsafePointer&lt;CChar>) -> Any!

Returns the metaclass definition of a specified class.

