

- Foundation
- NSIndexSet
-  makeIterator() 

Instance Method

# makeIterator()

Returns an *iterator* over the elements of this *sequence*.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> NSIndexSetIterator
```

## Discussion

Complexity: O(1).

## See Also

### Enumerating Indexes

func enumerate((Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block using each object in the index set.

func enumerate(options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block over the index set’s indexes, using the specified enumeration options.

func enumerate(in: NSRange, options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block using the indexes in the specified range, using the specified enumeration options.

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

