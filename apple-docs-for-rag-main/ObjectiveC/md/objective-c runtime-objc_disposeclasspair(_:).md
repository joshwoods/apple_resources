

- Objective-C Runtime
-  objc_disposeClassPair(\_:) 

Function

# objc_disposeClassPair(\_:)

Destroys a class and its associated metaclass.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_disposeClassPair(_ cls: AnyClass)
```

## Parameters 

`cls`  

The class to be destroyed. This class must have been allocated using objc_allocateClassPair(_:_:_:).

## Discussion

Do not call this function if instances of the `cls` class or any subclass exist.

## See Also

### Adding Classes

func objc_allocateClassPair(AnyClass?, UnsafePointer&lt;CChar>, Int) -> AnyClass?

Creates a new class and metaclass.

func objc_registerClassPair(AnyClass)

Registers a class that was allocated using objc_allocateClassPair(_:_:_:).

func objc_duplicateClass(AnyClass, UnsafePointer&lt;CChar>, Int) -> AnyClass

Used by Foundation’s Key-Value Observing.

