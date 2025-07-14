

- Core Services
- Search Kit
-  SKDocumentCreate(\_:\_:\_:) 

Function

# SKDocumentCreate(\_:\_:\_:)

Creates a document URL object (of type `SKDocument`) based on a scheme, parent, and name.

macOS 10.3+

``` source
func SKDocumentCreate(
    _ inScheme: CFString!,
    _ inParent: SKDocument!,
    _ inName: CFString!
) -> Unmanaged!
```

## Parameters 

`inScheme`  

The scheme to use—analogous to the scheme of a URL. Only documents referenced with the “`file`” scheme can be read by the SKIndexAddDocument(_:_:_:_:) function. The scheme can be anything you like if you use the SKIndexAddDocumentWithText(_:_:_:_:) function. The scheme can be `NULL`, in which case it will be set to be the same scheme as the document URL object’s parent. For more information on schemes, see http://www.iana.org/assignments/uri-schemes.html.

`inParent`  

The document URL object one step up in the document hierarchy. Can be `NULL`.

`inName`  

The name of the document that you’re creating a document URL object for. For the “`file`” scheme, it is the name of the file or the container, not its path. The path can be constructed by following parent links. The maximum length for a document name is 256 bytes.

## Return Value

The new document URL object, or `NULL` on failure.

## Discussion

The new document URL object’s parent can be `NULL`, but you must specify either a scheme or a parent. When your application no longer needs the document URL object, dispose of it by calling CFRelease.

## See Also

### Working with Documents and Terms

func SKDocumentCreateWithURL(CFURL!) -> Unmanaged&lt;SKDocument>!

Creates a document URL object (of type `SKDocument`) from a CFURL object.

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

