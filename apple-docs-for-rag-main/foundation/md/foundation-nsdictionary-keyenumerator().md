

- Foundation
- NSDictionary
-  keyEnumerator() 

Instance Method

# keyEnumerator()

Provides an enumerator to access the keys in the dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keyEnumerator() -> NSEnumerator
```

## Return Value

An enumerator object that lets you access each key in the dictionary.

## Discussion

Here’s how you might use this method.

- Swift
- Objective-C

```
let enumerator = myDictionary.keyEnumerator()

while let key = enumerator.nextObject() {
    /* code that uses the returned key */
}

```

```
NSEnumerator *enumerator = [myDictionary keyEnumerator];
id key;

while ((key = [enumerator nextObject])) {
    /* code that uses the returned key */
}
```

If you use this method with instances of mutable subclasses of NSDictionary, your code should not modify the entries during enumeration. If you intend to modify the entries, use the allKeys property to create a snapshot of the dictionary’s keys. Then use this snapshot to traverse the entries, modifying them along the way.

If you want to enumerate the dictionary’s values rather than its keys, use the objectEnumerator() method.

### Special Considerations

It is more efficient to use the fast enumeration protocol (see NSFastEnumeration) than this method. Fast enumeration is available in macOS 10.5 and later and iOS 2.0 and later.

## See Also

### Enumerating Dictionaries

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each value in the dictionary.

func enumerateKeysAndObjects((Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary.

func enumerateKeysAndObjects(options: NSEnumerationOptions, using: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary, with options specifying how the enumeration is performed.

func makeIterator() -> NSDictionary.Iterator

Returns an iterator over the elements of this sequence.

