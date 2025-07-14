

- Foundation
- NSPointerArray
-  removePointer(at:) 

Instance Method

# removePointer(at:)

Removes the pointer at a given index.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removePointer(at index: Int)
```

## Parameters 

`index`  

The index of an element in the receiver. This value must be less than the count of the receiver.

## Discussion

Elements above `index`, including `NULL` values, slide lower.

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

func insertPointer(UnsafeMutableRawPointer?, at: Int)

Inserts a pointer at a given index.

func replacePointer(at: Int, withPointer: UnsafeMutableRawPointer?)

Replaces the pointer at a given index.

func compact()

Removes `NULL` values from the receiver.

