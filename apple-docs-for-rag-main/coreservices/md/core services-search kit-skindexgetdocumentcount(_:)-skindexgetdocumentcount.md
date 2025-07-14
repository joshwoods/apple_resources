

- Core Services
- Search Kit
-  SKIndexGetDocumentCount(\_:) 

Function

# SKIndexGetDocumentCount(\_:)

Gets the total number of documents represented in an index.

macOS 10.3+

``` source
func SKIndexGetDocumentCount(_ inIndex: SKIndex!) -> CFIndex
```

## Parameters 

`inIndex`  

The index whose document URL objects (of type `SKDocument`) you want to count.

## Return Value

A `CFIndex` object containing the number of document URL objects (of type `SKDocument`) in the index. On failure, returns 0.

## Discussion

Document URL objects (of type `SKDocument`) added to an index have an indexing state of `kSKDocumentStateIndexed`. See the SKDocumentIndexState enumeration.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

### Special Considerations

In the current implementation of Search Kit, `SKIndexGetDocumentCount` returns the number of documents represented in the on-disk index. If your application has added document URL objects to the index but has not yet called SKIndexFlush(_:), the document count may not be correct.

## See Also

### Managing Indexes

func SKIndexAddDocumentWithText(SKIndex!, SKDocument!, CFString!, Bool) -> Bool

Adds a document URL (`SKDocument`) object, and the associated document’s textual content, to an index.

func SKIndexAddDocument(SKIndex!, SKDocument!, CFString!, Bool) -> Bool

Adds location information for a file-based document, and the document’s textual content, to an index.

func SKIndexFlush(SKIndex!) -> Bool

Invokes all pending updates associated with an index and commits them to backing store.

func SKIndexCompact(SKIndex!) -> Bool

Invokes all pending updates associated with an index, compacts the index if compaction is needed, and commits all changes to backing store.

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

