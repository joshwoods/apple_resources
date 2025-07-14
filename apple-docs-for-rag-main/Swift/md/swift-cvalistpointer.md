

- Swift
-  CVaListPointer 

Structure

# CVaListPointer

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct CVaListPointer
```

## Mentioned in 

Using Imported C Functions in Swift

## Topics

### Default Implementations

CustomDebugStringConvertible Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible

## See Also

### C Variadic Functions

func withVaList&lt;R>([any CVarArg], (CVaListPointer) -> R) -> R

Invokes the given closure with a C `va_list` argument derived from the given array of arguments.

protocol CVarArg

A type whose instances can be encoded, and appropriately passed, as elements of a C `va_list`.

func getVaList([any CVarArg]) -> CVaListPointer

Returns a `CVaListPointer` that is backed by autoreleased storage, built from the given array of arguments.

