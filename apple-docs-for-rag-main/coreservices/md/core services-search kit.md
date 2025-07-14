

- Core Services
-  Search Kit 

API Collection

# Search Kit

Index and search natural language documents.

## Overview

Search Kit is a powerful and streamlined C language framework for indexing and searching text in most human languages. It provides fast information retrieval in System Preferences, Address Book, Help Viewer, and Xcode. Apple’s Spotlight technology is built on top of Search Kit to provide content searching in Finder, Mail, and the Spotlight menu.

You can use Search Kit or Spotlight to provide similar functionality and powerful information-access capabilities within your Mac OS X application. The Search Kit API is appropriate when you want your application to have full control over indexing and searching, and when your focus is file content. Search Kit is thread-safe and works with Cocoa, Carbon, and command-line tools.

Beginning with Mac OS X version 10.4, Search Kit supports phrase searches, prefix/suffix/substring searches, improved Boolean searches, and improved relevance ranking. Search Kit now uses Spotlight’s metadata importers when indexing documents, and takes advantage of any additional importers available on a system. Searching and indexing are much faster with Search Kit’s new asynchronous search APIs. And, starting in Mac OS X v10.4, Search Kit provides a summarization API that supplants Find By Content.

### Overview

Search Kit is a powerful and streamlined C language framework for indexing and searching text in most human languages. It provides fast information retrieval in System Preferences, Address Book, Help Viewer, and Xcode. Apple’s Spotlight technology is built on top of Search Kit to provide content searching in Finder, Mail, and the Spotlight menu.

You can use Search Kit or Spotlight to provide similar functionality and powerful information-access capabilities within your Mac app. Search Kit is appropriate when you want your application to have full control over indexing and searching, and when your focus is file content. Search Kit is thread-safe and works with Cocoa and command-line tools.

Search Kit supports phrase searches, prefix/suffix/substring searches, Boolean searches, summarization, and relevance ranking. Search Kit uses Spotlight’s metadata importers when indexing documents and takes advantage of any additional importers available on a system.

## Topics

### Creating, Opening, and Closing Indexes

Search Kit performs its searches not on documents but on its indexes of documents. The functions in this group let your application create memory-based and persistent indexes. Indexes are initially empty. Functions in Managing Indexes let you add document content to these indexes.

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

func SKIndexGetIndexType(SKIndex!) -> SKIndexType

Gets the category of an index.

func SKIndexGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit indexes.

### Managing Indexes

The functions in this section let your application add document content to (and remove document content from) indexes, work with memory- and disk-based indexes, and retrieve metadata from indexes.

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

### Working With Text Importers

Search Kit can import the textual content of file-based documents into indexes using the Spotlight metadata importers.

func SKLoadDefaultExtractorPlugIns()

Tells Search Kit to use the Spotlight metadata importers.

### Working with Documents and Terms

From Search Kit’s perspective, a document is anything that contains text—an RTF document, a PDF file, a Mail message, an Address Book entry, an Internet URL, the result of a database query, and so on.

The functions in this section let your application create new document URL objects (SKDocumentRefs), retrieve metadata from documents, get information on document hierarchies, and work with documents and their terms in the context of Search Kit indexes.

func SKDocumentCreateWithURL(CFURL!) -> Unmanaged&lt;SKDocument>!

Creates a document URL object (of type `SKDocument`) from a CFURL object.

func SKDocumentCreate(CFString!, SKDocument!, CFString!) -> Unmanaged&lt;SKDocument>!

Creates a document URL object (of type `SKDocument`) based on a scheme, parent, and name.

func SKDocumentCopyURL(SKDocument!) -> Unmanaged&lt;CFURL>!

Builds a CFURL object from a document URL object (of type `SKDocument`).

func SKDocumentGetName(SKDocument!) -> Unmanaged&lt;CFString>!

Gets the name of a document URL object (of type `SKDocument`).

func SKDocumentGetParent(SKDocument!) -> Unmanaged&lt;SKDocument>!

Gets the parent of a document URL object (of type `SKDocument`).

func SKDocumentGetSchemeName(SKDocument!) -> Unmanaged&lt;CFString>!

Gets the scheme name for a document URL object (of type `SKDocument`).

func SKDocumentGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit document URL objects.

func SKIndexCopyDocumentForDocumentID(SKIndex!, SKDocumentID) -> Unmanaged&lt;SKDocument>!

Obtains a document URL object (of type `SKDocument`) from an index.

func SKIndexCopyInfoForDocumentIDs(SKIndex!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!, UnsafeMutablePointer&lt;SKDocumentID>!)

Gets document names and parent IDs based on document IDs.

func SKIndexCopyDocumentRefsForDocumentIDs(SKIndex!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Unmanaged&lt;SKDocument>?>!)

Gets document URL objects (of type `SKDocument`) based on document IDs.

func SKIndexCopyDocumentURLsForDocumentIDs(SKIndex!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!)

Gets document URLs based on document IDs.

func SKIndexCopyDocumentIDArrayForTermID(SKIndex!, CFIndex) -> Unmanaged&lt;CFArray>!

Obtains document IDs for documents that contain a given term.

func SKIndexCopyTermIDArrayForDocumentID(SKIndex!, SKDocumentID) -> Unmanaged&lt;CFArray>!

Obtains the IDs for the terms of an indexed document.

func SKIndexCopyTermStringForTermID(SKIndex!, CFIndex) -> Unmanaged&lt;CFString>!

Obtains a term, specified by ID, from an index.

func SKIndexGetTermIDForTermString(SKIndex!, CFString!) -> CFIndex

Gets the ID for a term in an index.

func SKIndexSetDocumentProperties(SKIndex!, SKDocument!, CFDictionary!)

Sets the application-defined properties of a document URL object (of type `SKDocument`).

func SKIndexCopyDocumentProperties(SKIndex!, SKDocument!) -> Unmanaged&lt;CFDictionary>!

Obtains the application-defined properties of an indexed document.

func SKIndexGetDocumentState(SKIndex!, SKDocument!) -> SKDocumentIndexState

Gets the current indexing state of a document URL object (of type `SKDocument`) in an index.

func SKIndexGetDocumentTermCount(SKIndex!, SKDocumentID) -> CFIndex

Gets the number of terms for a document in an index.

func SKIndexGetDocumentTermFrequency(SKIndex!, SKDocumentID, CFIndex) -> CFIndex

Gets the number of occurrences of a term in a document.

func SKIndexGetTermDocumentCount(SKIndex!, CFIndex) -> CFIndex

Gets the number of documents containing a given term represented in an index.

func SKIndexGetDocumentID(SKIndex!, SKDocument!) -> SKDocumentID

Gets the ID of a document URL object (of type `SKDocument`) in an index.

### Fast Asynchronous Searching

func SKSearchCreate(SKIndex!, CFString!, SKSearchOptions) -> Unmanaged&lt;SKSearch>!

Creates an asynchronous search object for querying an index, and initiates search.

func SKSearchFindMatches(SKSearch!, CFIndex, UnsafeMutablePointer&lt;SKDocumentID>!, UnsafeMutablePointer&lt;Float>!, CFTimeInterval, UnsafeMutablePointer&lt;CFIndex>!) -> Bool

Extracts search result information from a search object.

func SKSearchCancel(SKSearch!)

Cancels an asynchronous search request.

func SKSearchGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit search objects.

### Working With Summarization

Search Kit’s Summarization functions supplant those in Apple’s Find by Content API.

func SKSummaryCreateWithString(CFString!) -> Unmanaged&lt;SKSummary>!

Creates a summary object based on a text string.

func SKSummaryGetSentenceSummaryInfo(SKSummary!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Gets detailed information about a body of text for constructing a custom sentence-based summary string.

func SKSummaryGetParagraphSummaryInfo(SKSummary!, CFIndex, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!) -> CFIndex

Gets detailed information about a body of text for constructing a custom paragraph-based summary string.

func SKSummaryGetSentenceCount(SKSummary!) -> CFIndex

Gets the number of sentences in a summarization object.

func SKSummaryGetParagraphCount(SKSummary!) -> CFIndex

Gets the number of paragraphs in a summarization object.

func SKSummaryCopySentenceAtIndex(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a specified sentence from the text in a summarization object.

func SKSummaryCopyParagraphAtIndex(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a specified paragraph from the text in a summarization object.

func SKSummaryCopySentenceSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of sentences.

func SKSummaryCopyParagraphSummaryString(SKSummary!, CFIndex) -> Unmanaged&lt;CFString>!

Gets a text string consisting of a summary with, at most, the requested number of paragraphs.

func SKSummaryGetTypeID() -> CFTypeID

Gets the type identifier for Search Kit summarization objects.

### Callbacks

Developers should avoid using the callbacks listed in this section; instead, use SKSearchCreate(_:_:_:) and SKSearchFindMatches(_:_:_:_:_:_:).

typealias SKSearchResultsFilterCallBack

Deprecated. Use `SKSearchCreate` and `SKSearchFindMatches` instead, which do not use a callback.

### Data Types

typealias SKDocument

Defines an opaque data type representing a document’s URL.

class SKIndexDocumentIterator

Defines an opaque data type representing an index-based document iterator.

class SKIndex

Defines an opaque data type representing an index.

class SKSearch

Defines an opaque data type representing an asynchronous search.

class SKSummary

Defines an opaque data type representing summarization information.

typealias SKDocumentID

Defines an opaque data type representing a lightweight document identifier.

class SKSearchResults

Deprecated. Use asynchronous searching with SKSearchCreate instead, which does not employ search groups.

class SKSearchGroup

Deprecated. Use asynchronous searching with SKSearchCreate instead, which does not employ search groups.

### Constants

Text Analysis Keys

Each of these constants is an optional key in a Search Kit index’s text analysis properties dictionary. The constant descriptions describe the corresponding values for each of these keys. These keys are declared in the `Analysis.h` header file.

struct SKDocumentIndexState

The indexing state of a document.

typealias SKSearchOptions

Specifies the search options available for the SKSearchCreate(_:_:_:) function.

struct SKIndexType

Specifies the category of an index.

struct SKSearchType

Search Kit ignores the constants in this group. Use asynchronous searching with `SKSearchCreate` instead, which uses query syntax to determine search type.

var kSKDocumentStateAddPending: SKDocumentIndexState

Specifies that the document is not in the index but will be added after the index is flushed or closed.

var kSKDocumentStateDeletePending: SKDocumentIndexState

Specifies that the document is in the index but will be deleted after the index is flushed or closed.

var kSKDocumentStateIndexed: SKDocumentIndexState

Specifies that the document is indexed.

var kSKDocumentStateNotIndexed: SKDocumentIndexState

Specifies that the document is not indexed.

var kSKIndexInverted: SKIndexType

Specifies an inverted index, mapping terms to documents.

var kSKIndexInvertedVector: SKIndexType

Specifies an index type with all the capabilities of an inverted and a vector index.

var kSKIndexUnknown: SKIndexType

Specifies an unknown index type.

var kSKIndexVector: SKIndexType

Specifies a vector index, mapping documents to terms.

var kSKSearchBooleanRanked: SKSearchType

Deprecated. Specifies a query that can include Boolean operators including `'|'`, `'&'`, `'!'`, `'('`, and `')'`.

var kSKSearchPrefixRanked: SKSearchType

Deprecated. Specifies a prefix-based search, which matches terms that begin with the query string.

var kSKSearchRanked: SKSearchType

Deprecated. Specifies a basic ranked search.

var kSKSearchRequiredRanked: SKSearchType

Deprecated. Specifies a query that can include required (`'+'`) or excluded (`'-'`) terms.

## See Also

### Related Documentation

Search Kit Programming Guide

