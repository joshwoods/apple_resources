

- Objective-C Runtime
-  ivar_getTypeEncoding(\_:) 

Function

# ivar_getTypeEncoding(\_:)

Returns the type string of an instance variable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func ivar_getTypeEncoding(_ v: Ivar) -> UnsafePointer?
```

## Return Value

A C string containing the instance variable’s type encoding.

## Discussion

For possible values, see Objective-C Runtime Programming Guide \> Type Encodings.

## See Also

### Working with Instance Variables

func ivar_getName(Ivar) -> UnsafePointer&lt;CChar>?

Returns the name of an instance variable.

func ivar_getOffset(Ivar) -> Int

Returns the offset of an instance variable.

