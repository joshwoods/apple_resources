

- Objective-C Runtime
-  objc_registerClassPair(\_:) 

Function

# objc_registerClassPair(\_:)

Registers a class that was allocated using objc_allocateClassPair(_:_:_:).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_registerClassPair(_ cls: AnyClass)
```

## Parameters 

`cls`  

The class you want to register.

## See Also

### Adding Classes

func objc_allocateClassPair(AnyClass?, UnsafePointer&lt;CChar>, Int) -> AnyClass?

Creates a new class and metaclass.

func objc_disposeClassPair(AnyClass)

Destroys a class and its associated metaclass.

func objc_duplicateClass(AnyClass, UnsafePointer&lt;CChar>, Int) -> AnyClass

Used by Foundation’s Key-Value Observing.

