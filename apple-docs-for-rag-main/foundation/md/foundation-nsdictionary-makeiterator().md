

- Foundation
- NSDictionary
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the elements of this sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> NSDictionary.Iterator
```

## Discussion

Complexity: O(1).

## See Also

### Enumerating Dictionaries

func keyEnumerator() -> NSEnumerator

Provides an enumerator to access the keys in the dictionary.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each value in the dictionary.

func enumerateKeysAndObjects((Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary.

func enumerateKeysAndObjects(options: NSEnumerationOptions, using: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary, with options specifying how the enumeration is performed.

