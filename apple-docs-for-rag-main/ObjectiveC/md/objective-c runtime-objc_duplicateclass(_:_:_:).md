

- Objective-C Runtime
-  objc_duplicateClass(\_:\_:\_:) 

Function

# objc_duplicateClass(\_:\_:\_:)

Used by Foundation’s Key-Value Observing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_duplicateClass(
    _ original: AnyClass,
    _ name: UnsafePointer,
    _ extraBytes: Int
) -> AnyClass
```

## Discussion

Do not call this function yourself.

## See Also

### Adding Classes

func objc_allocateClassPair(AnyClass?, UnsafePointer&lt;CChar>, Int) -> AnyClass?

Creates a new class and metaclass.

func objc_disposeClassPair(AnyClass)

Destroys a class and its associated metaclass.

func objc_registerClassPair(AnyClass)

Registers a class that was allocated using objc_allocateClassPair(_:_:_:).

