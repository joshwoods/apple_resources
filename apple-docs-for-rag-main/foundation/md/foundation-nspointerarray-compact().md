

- Foundation
- NSPointerArray
-  compact() 

Instance Method

# compact()

Removes `NULL` values from the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compact()
```

## See Also

### Managing the Collection

var count: Int

The number of elements in the receiver.

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

