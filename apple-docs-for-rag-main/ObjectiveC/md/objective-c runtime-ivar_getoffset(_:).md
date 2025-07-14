

- Objective-C Runtime
-  ivar_getOffset(\_:) 

Function

# ivar_getOffset(\_:)

Returns the offset of an instance variable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func ivar_getOffset(_ v: Ivar) -> Int
```

## Discussion

For instance variables of type `id` or other object types, call object_getIvar(_:_:) and object_setIvar(_:_:_:) instead of using this offset to access the instance variable data directly.

## See Also

### Working with Instance Variables

func ivar_getName(Ivar) -> UnsafePointer&lt;CChar>?

Returns the name of an instance variable.

func ivar_getTypeEncoding(Ivar) -> UnsafePointer&lt;CChar>?

Returns the type string of an instance variable.

