

- Swift
- Hasher
-  combine(\_:) 

Instance Method

# combine(\_:)

Adds the given value to this hasher, mixing its essential parts into the hasher state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func combine(_ value: H) where H : Hashable
```

## Parameters 

`value`  

A value to add to the hasher.

## See Also

### Adding Values

func combine(bytes: UnsafeRawBufferPointer)

Adds the contents of the given buffer to this hasher, mixing it into the hasher state.

