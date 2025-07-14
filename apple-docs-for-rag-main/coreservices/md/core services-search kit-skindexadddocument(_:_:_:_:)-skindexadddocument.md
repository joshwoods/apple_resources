

- Core Services
- Search Kit
-  SKIndexAddDocument(\_:\_:\_:\_:) 

Function

# SKIndexAddDocument(\_:\_:\_:\_:)

Adds location information for a file-based document, and the document’s textual content, to an index.

macOS 10.3+

``` source
func SKIndexAddDocument(
    _ inIndex: SKIndex!,
    _ inDocument: SKDocument!,
    _ inMIMETypeHint: CFString!,
    _ inCanReplace: Bool
) -> Bool
```

## Parameters 

`inIndex`  

The index to which you are adding the document URL object (`SKDocument`).

`inDocument`  

The document URL object (of type `SKDocument`) , containing a file-based document’s location information, to add to the index. You can release the document URL object immediately after adding it to the index.

`inMIMETypeHint`  

The MIME type hint for the specified file-based document. Can be `NULL`. In Search Kit, common MIME type hints include `text/plain`, `text/rtf`, `text/html`, `text/pdf`, and `application/msword`.

Specify a MIME type hint to help Spotlight determine which of its metadata importers to use when Search Kit is indexing a file-based document. Search Kit uses filename extensions and type/creator codes in attempting to determine file types when indexing files. See SKLoadDefaultExtractorPlugIns(). You can circumvent Search Kit’s file type determination process, or override it, by using a MIME type hint.

`inCanReplace`  

A Boolean value specifying whether Search Kit will overwrite a document’s index entry (`true`, indicated by `1` or `kCFBooleanTrue`), or retain the entry if it exists (`false`, indicated by `0` or `kCFBoolenFalse`).

## Return Value

A Boolean value of `true` on success, or `false` on failure. Also returns `false` if the document has an entry in the index and `inCanReplace` is set to `false`.

## Discussion

The document scheme must be of type “`file`” to use this function. If it’s not, call SKIndexAddDocumentWithText(_:_:_:_:) instead. For more information on schemes, see http://www.iana.org/assignments/uri-schemes.html.

This function uses the referenced document and the optional MIME type hint to get the document’s textual content using the Spotlight metadata importers. If you do not supply a MIME type hint, Spotlight’s importers will use filename extensions and type/creator codes to guess file types.

Search Kit indexes any nonexecutable file associated with a document URL object (of type `SKDocument`) that you hand to this function, even nontext files such as images. Your application takes responsibility for ensuring that the document URL objects you pass to `SKIndexAddDocument` are in fact the locations of files you want to index.

If your application did not call SKLoadDefaultExtractorPlugIns(), Search Kit indexes the first 10 MB of a document. Otherwise, Search Kit indexes the entire document up to the index file size limit of 4 GB.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

A single Search Kit index can hold up to 4 billion document URL objects and their associated textual content.

### Special Considerations

In the current implementation of Search Kit, some functions do not provide expected results unless you follow `SKIndexAddDocument` with a call to SKIndexFlush(_:). The affected functions include SKIndexGetDocumentCount(_:), SKIndexGetDocumentTermCount(_:_:), SKIndexGetDocumentTermFrequency(_:_:_:), and SKIndexGetTermDocumentCount(_:_:). However, in typical use this won’t be an issue, because applications call these functions after a search, and you must call `SKIndexFlush` before a search.

## See Also

### Managing Indexes

func SKIndexAddDocumentWithText(SKIndex!, SKDocument!, CFString!, Bool) -> Bool

Adds a document URL (`SKDocument`) object, and the associated document’s textual content, to an index.

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

