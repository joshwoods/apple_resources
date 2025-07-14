

- Core Services
- File Metadata
- MDItem
-  MDItemCreate(\_:\_:) 

Function

# MDItemCreate(\_:\_:)

Creates an MDItem object for a file at the specified path.

macOS 10.4+

``` source
func MDItemCreate(
    _ allocator: CFAllocator!,
    _ path: CFString!
) -> MDItem!
```

## Parameters 

`allocator`  

The `CFAllocator` object to be used to allocate memory for the new object. Pass `NULL` or `kCFAllocatorDefault` to use the current default allocator.

`path`  

A path to the file from which to create the `MDItem`. The path must exist.

## Return Value

An `MDItem` object or `NULL` if there was a problem creating the object.

## Discussion

Returns a metadata item for the given URL.

### Special Considerations

In macOS 10.5 and later MDItemRefs may or may not be uniqued. You should always use `CFEqual` for comparison.

Prior to OS X v 10.5 items were guaranteed to be unique and == could or `CFEqual` could be used for the comparison.

## See Also

### Creating an MDItem

func MDItemCreateWithURL(CFAllocator!, CFURL!) -> MDItem!

Creates an MDItem object for a file at the specified file URL.

