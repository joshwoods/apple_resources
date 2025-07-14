

- Core Services
- Search Kit
-  SKIndexOpenWithData(\_:\_:) 

Function

# SKIndexOpenWithData(\_:\_:)

Opens an existing, named index for searching only.

macOS 10.3+

``` source
func SKIndexOpenWithData(
    _ inData: CFData!,
    _ inIndexName: CFString!
) -> Unmanaged!
```

## Parameters 

`inData`  

The index to open.

`inIndexName`  

The name of the index. Can be `NULL`, in which case this function attempts to open the index with the default name of `IADefaultIndex`.

## Return Value

The named index, or `NULL` on failure.

## Discussion

An index opened by `SKIndexOpenWithData` can be searched but not updated. To open an index for updating, use SKIndexOpenWithMutableData(_:_:).

If `inIndexName` is `NULL` and `inData` does not contain an index with the default name, this function returns `NULL`.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

A call to `SKIndexOpenWithData` retains the opened index. When your application no longer needs the index, dispose of it by calling SKIndexClose(_:).

### Special Considerations

You cannot use CFMakeCollectable with `SKIndex` objects.

## See Also

### Creating, Opening, and Closing Indexes

func SKIndexCreateWithURL(CFURL!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index in a file whose location is specified with a CFURL object.

func SKIndexCreateWithMutableData(CFMutableData!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index stored in a `CFMutableDataRef` object.

func SKIndexOpenWithMutableData(CFMutableData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching and updating.

func SKIndexOpenWithURL(CFURL!, CFString!, Bool) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index stored in a file whose location is specified with a CFURL object.

func SKIndexClose(SKIndex!)

Closes an index.

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

