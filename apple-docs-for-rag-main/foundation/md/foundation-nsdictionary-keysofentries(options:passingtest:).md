

- Foundation
- NSDictionary
-  keysOfEntries(options:passingTest:) 

Instance Method

# keysOfEntries(options:passingTest:)

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keysOfEntries(
    options opts: NSEnumerationOptions = [],
    passingTest predicate: (Any, Any, UnsafeMutablePointer) -> Bool
) -> Set
```

## Parameters 

`opts`  

A bit mask of enumeration options.

`predicate`  

A block object that specifies constraints for values in the dictionary.

## Return Value

The set of keys whose corresponding value satisfies `predicate`.

## See Also

### Related Documentation

func enumerateKeysAndObjects(options: NSEnumerationOptions, using: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary, with options specifying how the enumeration is performed.

### Filtering Dictionaries

func keysOfEntries(passingTest: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

