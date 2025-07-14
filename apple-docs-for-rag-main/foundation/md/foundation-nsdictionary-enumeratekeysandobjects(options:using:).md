

- Foundation
- NSDictionary
-  enumerateKeysAndObjects(options:using:) 

Instance Method

# enumerateKeysAndObjects(options:using:)

Applies a given block object to the entries of the dictionary, with options specifying how the enumeration is performed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateKeysAndObjects(
    options opts: NSEnumerationOptions = [],
    using block: (Any, Any, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`opts`  

Enumeration options.

`block`  

A block object to operate on entries in the dictionary.

## Discussion

If the block sets `*stop` to true, the enumeration stops.

## See Also

### Enumerating Dictionaries

func keyEnumerator() -> NSEnumerator

Provides an enumerator to access the keys in the dictionary.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each value in the dictionary.

func enumerateKeysAndObjects((Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary.

func makeIterator() -> NSDictionary.Iterator

Returns an iterator over the elements of this sequence.

