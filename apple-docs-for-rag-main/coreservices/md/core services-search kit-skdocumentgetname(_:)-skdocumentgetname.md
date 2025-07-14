

- Core Services
- Search Kit
-  SKDocumentGetName(\_:) 

Function

# SKDocumentGetName(\_:)

Gets the name of a document URL object (of type `SKDocument`).

macOS 10.3+

``` source
func SKDocumentGetName(_ inDocument: SKDocument!) -> Unmanaged!
```

## Parameters 

`inDocument`  

The document URL object whose name you want to get.

## Return Value

A CFString object containing the document URL object’s name, or `NULL` on failure.

## See Also

### Working with Documents and Terms

func SKDocumentCreateWithURL(CFURL!) -> Unmanaged&lt;SKDocument>!

Creates a document URL object (of type `SKDocument`) from a CFURL object.

func SKDocumentCreate(CFString!, SKDocument!, CFString!) -> Unmanaged&lt;SKDocument>!

Creates a document URL object (of type `SKDocument`) based on a scheme, parent, and name.

func SKDocumentCopyURL(SKDocument!) -> Unmanaged&lt;CFURL>!

Builds a CFURL object from a document URL object (of type `SKDocument`).

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

