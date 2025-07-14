

- Foundation
- NSDictionary
-  keysOfEntries(passingTest:) 

Instance Method

# keysOfEntries(passingTest:)

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keysOfEntries(passingTest predicate: (Any, Any, UnsafeMutablePointer) -> Bool) -> Set
```

## Parameters 

`predicate`  

A block object that specifies constraints for values in the dictionary.

## Return Value

The set of keys whose corresponding value satisfies `predicate`.

## See Also

### Related Documentation

func enumerateKeysAndObjects((Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary.

### Filtering Dictionaries

func keysOfEntries(options: NSEnumerationOptions, passingTest: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

