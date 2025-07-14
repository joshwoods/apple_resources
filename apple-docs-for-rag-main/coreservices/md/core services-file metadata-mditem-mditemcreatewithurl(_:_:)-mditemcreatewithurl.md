

- Core Services
- File Metadata
- MDItem
-  MDItemCreateWithURL(\_:\_:) 

Function

# MDItemCreateWithURL(\_:\_:)

Creates an MDItem object for a file at the specified file URL.

macOS 10.6+

``` source
func MDItemCreateWithURL(
    _ allocator: CFAllocator!,
    _ url: CFURL!
) -> MDItem!
```

## Parameters 

`allocator`  

The `CFAllocator` object to be used to allocate memory for the new object. Pass `NULL` or `kCFAllocatorDefault` to use the current default allocator.

`url`  

A file URL to the file from which to create the `MDItem`. The file must exist.

## Return Value

An `MDItem` object or `NULL` if there was a problem creating the object.

## Discussion

Returns a metadata item for the given URL.

### Special Considerations

In macOS 10.5 and later MDItemRefs may or may not be uniqued. You should always use `CFEqual` for comparison.

Prior to OS X v 10.5 items were guaranteed to be unique and == could or `CFEqual` could be used for the comparison.

## See Also

### Creating an MDItem

func MDItemCreate(CFAllocator!, CFString!) -> MDItem!

Creates an MDItem object for a file at the specified path.

