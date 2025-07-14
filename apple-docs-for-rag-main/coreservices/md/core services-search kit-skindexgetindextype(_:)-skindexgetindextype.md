

- Core Services
- Search Kit
-  SKIndexGetIndexType(\_:) 

Function

# SKIndexGetIndexType(\_:)

Gets the category of an index.

macOS 10.3+

``` source
func SKIndexGetIndexType(_ inIndex: SKIndex!) -> SKIndexType
```

## Parameters 

`inIndex`  

The index whose category you want to know.

## Return Value

The category of the index. See the SKIndexType enumeration for a list of the various index categories. On failure, returns a value of `kSKIndexUnknown`.

## Discussion

As described in SKIndexType, Search Kit offers four categories of index, each optimized for one or more types of searching.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

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

func SKIndexOpenWithURL(CFURL!, CFString!, Bool) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index stored in a file whose location is specified with a CFURL object.

func SKIndexClose(SKIndex!)

Closes an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

