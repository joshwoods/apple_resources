

- Foundation
- NSPointerArray
-  count 

Instance Property

# count

The number of elements in the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var count: Int { get set }
```

## Discussion

If you increase the `count`, `NULL` values are added. If you decrease the `count`, elements at indexes `count` and greater are removed.

## See Also

### Managing the Collection

var allObjects: [Any]

All the objects in the receiver.

func pointer(at: Int) -> UnsafeMutableRawPointer?

Returns the pointer at a given index.

func addPointer(UnsafeMutableRawPointer?)

Adds a given pointer to the receiver.

func removePointer(at: Int)

Removes the pointer at a given index.

func insertPointer(UnsafeMutableRawPointer?, at: Int)

Inserts a pointer at a given index.

func replacePointer(at: Int, withPointer: UnsafeMutableRawPointer?)

Replaces the pointer at a given index.

func compact()

Removes `NULL` values from the receiver.

