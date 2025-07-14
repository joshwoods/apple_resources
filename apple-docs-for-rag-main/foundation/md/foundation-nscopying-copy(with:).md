

- Foundation
- NSCopying
-  copy(with:) 

Instance Method

# copy(with:)

Returns a new instance that’s a copy of the receiver.

iOS 1.0+iPadOS 1.0+Mac Catalyst 1.0+macOS 10.0+tvOS 1.0+visionOS 1.0+watchOS 1.0+

``` source
func copy(with zone: NSZone? = nil) -> Any
```

**Required**

## Parameters 

`zone`  

This parameter is ignored. Memory zones are no longer used by Objective-C.

## Discussion

The returned object is implicitly retained by the sender, who is responsible for releasing it. The copy returned is immutable if the consideration “immutable vs. mutable” applies to the receiving object; otherwise the exact nature of the copy is determined by the class.

## See Also

### Related Documentation

func mutableCopy(with: NSZone?) -> Any

Returns a new instance that’s a mutable copy of the receiver.

**Required**

func copy() -> Any

Returns the object returned by \`copy(with:)\`.

Advanced Memory Management Programming Guide

