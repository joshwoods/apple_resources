

- Core Services
- Search Kit
-  SKIndexDocumentIteratorCreate(\_:\_:) 

Function

# SKIndexDocumentIteratorCreate(\_:\_:)

Creates an index-based iterator for document URL objects (of type `SKDocument`) owned by a parent document URL object.

macOS 10.3+

``` source
func SKIndexDocumentIteratorCreate(
    _ inIndex: SKIndex!,
    _ inParentDocument: SKDocument!
) -> Unmanaged!
```

## Parameters 

`inIndex`  

The index you want to iterate across.

`inParentDocument`  

The document URL object that is the parent of the document URL objects you want to examine. Pass `NULL` to get the top item in an index. See SKDocument for a discussion of how to get the full URL for a document URL object.

## Return Value

An index-based document iterator.

## Discussion

When you want to iterate across all the documents represented in an index, use this function to create an iterator and then call SKIndexDocumentIteratorCopyNext(_:) in turn for each document URL object (of type `SKDocument`) in the index.

Document iterators iterate over a single level of an index. Your code is responsible for descending through a hierarchy of documents in an index.

Search Kit is thread-safe. You can use separate indexing and searching threads. Your application is responsible for ensuring that no more than one process is open at a time for writing to an index.

When your application no longer needs the iterator, dispose of it by calling CFRelease.

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

func SKIndexGetMaximumDocumentID(SKIndex!) -> SKDocumentID

Gets the highest-numbered document ID in an index.

func SKIndexGetMaximumTermID(SKIndex!) -> CFIndex

Gets the highest-numbered term ID in an index.

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

