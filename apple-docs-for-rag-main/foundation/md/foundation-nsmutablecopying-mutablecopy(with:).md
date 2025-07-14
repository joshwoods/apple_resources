

- Foundation
- NSMutableCopying
-  mutableCopy(with:) 

Instance Method

# mutableCopy(with:)

Returns a new instance that’s a mutable copy of the receiver.

iOS 1.0+iPadOS 1.0+Mac Catalyst 1.0+macOS 10.0+tvOS 1.0+visionOS 1.0+watchOS 1.0+

``` source
func mutableCopy(with zone: NSZone? = nil) -> Any
```

**Required**

## Parameters 

`zone`  

This parameter is ignored. Memory zones are no longer used by Objective-C.

## Discussion

The returned object is implicitly retained by the sender, which is responsible for releasing it. The copy returned is mutable whether the original is mutable or not.

## See Also

### Related Documentation

func copy(with: NSZone?) -> Any

Returns a new instance that’s a copy of the receiver.

**Required**

Advanced Memory Management Programming Guide

func mutableCopy() -> Any

Returns the object returned by \`mutableCopy(with:)\` where the zone is \`nil\`.

