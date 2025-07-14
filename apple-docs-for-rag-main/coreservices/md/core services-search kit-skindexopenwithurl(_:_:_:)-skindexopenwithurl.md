

- Core Services
- Search Kit
-  SKIndexOpenWithURL(\_:\_:\_:) 

Function

# SKIndexOpenWithURL(\_:\_:\_:)

Opens an existing, named index stored in a file whose location is specified with a CFURL object.

macOS 10.3+

``` source
func SKIndexOpenWithURL(
    _ inURL: CFURL!,
    _ inIndexName: CFString!,
    _ inWriteAccess: Bool
) -> Unmanaged!
```

## Parameters 

`inURL`  

The location of the index.

`inIndexName`  

The name of the index. Can be `NULL`, in which case this function attempts to open the index with the default name of `IADefaultIndex`.

`inWriteAccess`  

A Boolean value indicating whether the index is open for updating. To open an index for searching only, pass `false` (`0` or `kCFBoolenFalse`). To open it for searching and updating, pass `true` (`1` or `kCFBooleanTrue`).

## Return Value

The named index, or `NULL` on failure.

## Discussion

If `inIndexName` is `NULL` and `inData` does not contain an index with the default name, this function returns `NULL`.

A call to `SKIndexOpenWithURL` retains the opened index. When your application no longer needs the index, dispose of it by calling SKIndexClose(_:).

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

### Special Considerations

You cannot use CFMakeCollectable with `SKIndex` objects.

## See Also

### Creating, Opening, and Closing Indexes

func SKIndexCreateWithURL(CFURL!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index in a file whose location is specified with a CFURL object.

func SKIndexCreateWithMutableData(CFMutableData!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index stored in a `CFMutableDataRef` object.

func SKIndexOpenWithData(CFData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching only.

func SKIndexOpenWithMutableData(CFMutableData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching and updating.

func SKIndexClose(SKIndex!)

Closes an index.

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

