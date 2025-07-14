

- Objective-C Runtime
-  ivar_getName(\_:) 

Function

# ivar_getName(\_:)

Returns the name of an instance variable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func ivar_getName(_ v: Ivar) -> UnsafePointer?
```

## Return Value

A C string containing the instance variable’s name.

## See Also

### Working with Instance Variables

func ivar_getTypeEncoding(Ivar) -> UnsafePointer&lt;CChar>?

Returns the type string of an instance variable.

func ivar_getOffset(Ivar) -> Int

Returns the offset of an instance variable.

