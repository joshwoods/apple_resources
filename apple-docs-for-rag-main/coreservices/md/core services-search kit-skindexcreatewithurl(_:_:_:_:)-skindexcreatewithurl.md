

- Core Services
- Search Kit
-  SKIndexCreateWithURL(\_:\_:\_:\_:) 

Function

# SKIndexCreateWithURL(\_:\_:\_:\_:)

Creates a named index in a file whose location is specified with a CFURL object.

macOS 10.3+

``` source
func SKIndexCreateWithURL(
    _ inURL: CFURL!,
    _ inIndexName: CFString!,
    _ inIndexType: SKIndexType,
    _ inAnalysisProperties: CFDictionary!
) -> Unmanaged!
```

## Parameters 

`inURL`  

The location of the index.

`inIndexName`  

The name of the index. If you call this function with `inIndexName` set to `NULL`, Search Kit assigns the index the default index name `IADefaultIndex`. If you then attempt to create a second index in the same file without assigning a name, no second index is created and this function returns `NULL`. Search Kit does not currently support retrieving index names from an index.

`inIndexType`  

The index type. See SKIndexType.

`inAnalysisProperties`  

The text analysis properties dictionary, which optionally sets the minimum term length, stopwords, term substitutions, maximum unique terms to index, and proximity support (for phrase-based searches) when creating the index. See Text Analysis Keys. To get the analysis properties of an index, use the SKIndexGetAnalysisProperties(_:) function. The `inAnalysisProperties` parameter can be `NULL`, in which case Search Kit applies the default dictionary, which is `NULL`.

## Return Value

A unique reference to the newly created index.

## Discussion

`SKIndexCreateWithURL` creates an index in a file. Search Kit indexes are initially empty. Use this function when your application needs persistent storage of an index. To create a memory-based, nonpersistent index, use SKIndexCreateWithMutableData(_:_:_:_:).

A file can contain more than one index. To add a new index to an existing file, use the same value for `inURL` and supply a new name for `inIndexName`.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

When your application no longer needs the index, dispose of it by calling SKIndexClose(_:).

### Special Considerations

You cannot use CFMakeCollectable with `SKIndex` objects.

## See Also

### Creating, Opening, and Closing Indexes

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

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

