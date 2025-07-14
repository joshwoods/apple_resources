

- Core Services
- Search Kit
-  SKIndexGetMaximumDocumentID(\_:) 

Function

# SKIndexGetMaximumDocumentID(\_:)

Gets the highest-numbered document ID in an index.

macOS 10.3+

``` source
func SKIndexGetMaximumDocumentID(_ inIndex: SKIndex!) -> SKDocumentID
```

## Parameters 

`inIndex`  

An index.

## Return Value

A document ID object containing the highest-numbered document ID in the index.

## Discussion

Use this function with SKIndexGetDocumentCount(_:) to determine whether an index is fragmented and in need of compaction. See SKIndexCompact(_:).

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

### Version-Notes

In versions of macOS prior to OS X v10.4, the return type for `SKIndexGetMaximumDocumentID` was `CFIndex`. The return type in macOS 10.4 and later is `SKDocumentID`.

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

func SKIndexGetDocumentCount(SKIndex!) -> CFIndex

Gets the total number of documents represented in an index.

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

