

- Foundation
- NSIndexSet
-  enumerate(\_:) 

Instance Method

# enumerate(\_:)

Executes a given Block using each object in the index set.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerate(_ block: (Int, UnsafeMutablePointer) -> Void)
```

## Parameters 

`block`  

The Block to apply to elements in the set.

The Block takes two arguments:

idx  
The index of the object.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this Boolean to YES within the Block.

## Discussion

This method executes synchronously.

## See Also

### Enumerating Indexes

func enumerate(options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block over the index set’s indexes, using the specified enumeration options.

func enumerate(in: NSRange, options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block using the indexes in the specified range, using the specified enumeration options.

func makeIterator() -> NSIndexSetIterator

Returns an *iterator* over the elements of this *sequence*.

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

