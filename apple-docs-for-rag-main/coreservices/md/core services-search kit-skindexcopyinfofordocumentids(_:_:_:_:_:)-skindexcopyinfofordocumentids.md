

- Core Services
- Search Kit
-  SKIndexCopyInfoForDocumentIDs(\_:\_:\_:\_:\_:) 

Function

# SKIndexCopyInfoForDocumentIDs(\_:\_:\_:\_:\_:)

Gets document names and parent IDs based on document IDs.

macOS 10.4+

``` source
func SKIndexCopyInfoForDocumentIDs(
    _ inIndex: SKIndex!,
    _ inCount: CFIndex,
    _ inDocumentIDsArray: UnsafeMutablePointer!,
    _ outNamesArray: UnsafeMutablePointer?>!,
    _ outParentIDsArray: UnsafeMutablePointer!
)
```

## Parameters 

`inIndex`  

The index containing the document information.

`inCount`  

The number of document IDs in `inDocumentIDsArray`.

`inDocumentIDsArray`  

Points to an array of document IDs representing the documents whose names and parent IDs you want.

`outNamesArray`  

On input, a pointer to an array for document names. On output, points to the previously allocated array, which now contains the document names corresponding to the document IDs in `inDocumentIDsArray`. May be `NULL` on input if you don’t want to get the document names.

When finished with the names array, dispose of it by calling CFRelease on each array element.

`outParentIDsArray`  

On input, a pointer to an array for parent document IDs. On output, points to the previously allocated array, which now contains document IDs representing the parents of the documents whose IDs are in `inDocumentIDsArray`. May be `NULL` on input if you don’t want to get the parent document IDs.

## Discussion

The `SKIndexCopyInfoForDocumentIDs(_:_:_:_:_:)` function lets you get a batch of document names and parent document IDs in one step, based on a list of document IDs.

## See Also

### Working with Documents and Terms

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

