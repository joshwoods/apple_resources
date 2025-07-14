

- Core Services
- Search Kit
-  SKIndexAddDocumentWithText(\_:\_:\_:\_:) 

Function

# SKIndexAddDocumentWithText(\_:\_:\_:\_:)

Adds a document URL (`SKDocument`) object, and the associated document’s textual content, to an index.

macOS 10.3+

``` source
func SKIndexAddDocumentWithText(
    _ inIndex: SKIndex!,
    _ inDocument: SKDocument!,
    _ inDocumentText: CFString!,
    _ inCanReplace: Bool
) -> Bool
```

## Parameters 

`inIndex`  

The index to which you are adding the document URL object (`SKDocument`) .

`inDocument`  

The document URL (`SKDocument`) object to add.

`inDocumentText`  

The document text. Can be `NULL`.

`inCanReplace`  

A Boolean value specifying whether Search Kit will overwrite a document’s index entry (`true`, indicated by `1` or `kCFBooleanTrue`), or retain the entry if it exists (`false`, indicated by `0` or `kCFBoolenFalse`).

## Return Value

A Boolean value of `true` on success, or `false` on failure. Also returns `false` if the document has an entry in the index and `inCanReplace` is set to `false`.

## Discussion

Use this function to add the textual contents of arbitrary document types to an index. With this function, your application takes responsibility for getting textual content and handing it to the index as A `CFString` object. Because of this, your application can define what it considers to be a document—a database record, a tagged field in an XML document, an object in memory, a text file, and so on.

Search Kit will index any size text string that you give it, up to its 4 GB index file size limit.

To add the textual content of file-based documents to a Search Kit index, you can use this function or take advantage of Search Kit’s ability to locate and read certain on-disk, file-based document types—see SKIndexAddDocument(_:_:_:_:).

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

A single Search Kit index file can be up to 4 GB in size.

### Special Considerations

In OS X v10.3, some functions do not provide expected results unless you follow a call to `SKIndexAddDocumentWithText` with a call to SKIndexFlush(_:). The affected functions include SKIndexGetDocumentCount(_:), SKIndexGetDocumentTermCount(_:_:), SKIndexGetDocumentTermFrequency(_:_:_:), and SKIndexGetTermDocumentCount(_:_:). However, in typical use this won’t be an issue, because applications call these functions after a search, and you must call `SKIndexFlush` before a search.

## See Also

### Managing Indexes

func SKIndexAddDocument(SKIndex!, SKDocument!, CFString!, Bool) -> Bool

Adds location information for a file-based document, and the document’s textual content, to an index.

func SKIndexFlush(SKIndex!) -> Bool

Invokes all pending updates associated with an index and commits them to backing store.

func SKIndexCompact(SKIndex!) -> Bool

Invokes all pending updates associated with an index, compacts the index if compaction is needed, and commits all changes to backing store.

func SKIndexGetDocumentCount(SKIndex!) -> CFIndex

Gets the total number of documents represented in an index.

func SKIndexGetMaximumDocumentID(SKIndex!) -> SKDocumentID

Gets the highest-numbered document ID in an index.

func SKIndexGetMaximumTermID(SKIndex!) -> CFIndex

Gets the highest-numbered term ID in an index.

func SKIndexDocumentIteratorCreate(SKIndex!, SKDocument!) -> Unmanaged&lt;SKIndexDocumentIterator>!

Creates an index-based iterator for document URL objects (of type `SKDocument`) owned by a parent document URL object.

func SKIndexDocumentIteratorCopyNext(SKIndexDocumentIterator!) -> Unmanaged&lt;SKDocument>!

Obtains the next document URL object (of type `SKDocument`) from an index using a document iterator.

func SKIndexDocumentIteratorGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit document iterators.

func SKIndexGetAnalysisProperties(SKIndex!) -> Unmanaged&lt;CFDictionary>!

Gets the text analysis properties of an index.

func SKIndexMoveDocument(SKIndex!, SKDocument!, SKDocument!) -> Bool

Changes the parent of a document URL object (of type `SKDocument`) in an index.

func SKIndexRemoveDocument(SKIndex!, SKDocument!) -> Bool

Removes a document URL object (of type `SKDocument`) and its children, if any, from an index.

func SKIndexRenameDocument(SKIndex!, SKDocument!, CFString!) -> Bool

Changes the name of a document URL object (of type `SKDocument`) in an index.

func SKIndexSetMaximumBytesBeforeFlush(SKIndex!, CFIndex)

Not recommended. Sets the memory size limit for updates to an index, measured in bytes.

func SKIndexGetMaximumBytesBeforeFlush(SKIndex!) -> CFIndex

Not recommended. Gets the memory size limit for updates to an index, measured in bytes.

