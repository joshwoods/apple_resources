

- Core Services
- Search Kit
-  SKIndexCreateWithMutableData(\_:\_:\_:\_:) 

Function

# SKIndexCreateWithMutableData(\_:\_:\_:\_:)

Creates a named index stored in a `CFMutableDataRef` object.

macOS 10.3+

``` source
func SKIndexCreateWithMutableData(
    _ inData: CFMutableData!,
    _ inIndexName: CFString!,
    _ inIndexType: SKIndexType,
    _ inAnalysisProperties: CFDictionary!
) -> Unmanaged!
```

## Parameters 

`inData`  

An empty CFMutableData object to contain the index being created.

`inIndexName`  

The name of the index. If you call this function with `inIndexName` set to `NULL`, Search Kit assigns the index the default index name `IADefaultIndex`. If you then attempt to create a second index in the same file without assigning a name, no second index is created and this function returns `NULL`. Search Kit does not support retrieving index names from an index.

`inIndexType`  

The index type. See SKIndexType.

`inAnalysisProperties`  

The text analysis properties dictionary, which optionally sets the minimum term length, stopwords, term substitutions, maximum unique terms to index, and proximity support (for phrase-based searches) when creating the index. See Text Analysis Keys. The `inAnalysisProperties` parameter can be `NULL`, in which case Search Kit applies the default dictionary, which is `NULL`.

## Return Value

The newly created index.

## Discussion

`SKIndexCreateWithMutableData(_:_:_:_:)` creates an index in memory as a CFMutableData object. Search Kit indexes are initially empty. A memory-based index is useful for quick searching and when your application doesn’t need persistent storage. To create a disk-based, persistent index, use the SKIndexCreateWithURL(_:_:_:_:) function.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

This function retains the data object you provide in the `inData` parameter.

When your application no longer needs the index, dispose of it by calling SKIndexClose(_:).

### Special Considerations

You cannot use CFMakeCollectable with `SKIndex` objects.

## See Also

### Creating, Opening, and Closing Indexes

func SKIndexCreateWithURL(CFURL!, CFString!, SKIndexType, CFDictionary!) -> Unmanaged&lt;SKIndex>!

Creates a named index in a file whose location is specified with a CFURL object.

func SKIndexOpenWithData(CFData!, CFString!) -> Unmanaged&lt;SKIndex>!

Opens an existing, named index for searching only.

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

