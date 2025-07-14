

- Bundle Resources
- Information Property List
-  CFBundleDocumentTypes 

Property List Key

# CFBundleDocumentTypes

The document types supported by the bundle.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Name  
Document types

Type  

array of dictionaries

## Topics

### Property List Keys

CFBundleTypeIconFile

The icon to associate with the document type.

**Name:** Icon File Name

CFBundleTypeName

The abstract name for the document type.

**Name:** Document Type Name

CFBundleTypeRole

The app’s role with respect to the document type.

**Name:** Role

LSHandlerRank

The ranking of this app among apps that declare themselves as editors or viewers of the given file type.

**Name:** Handler rank

LSItemContentTypes

The document file types the app supports.

**Name:** Document Content Type UTIs

LSTypeIsPackage

A Boolean value indicating whether the document is distributed as a bundle.

**Name:** Document is a package or bundle

NSDocumentClass

The subclass used to create instances of this document.

**Name:** Cocoa NSDocument Class

NSExportableTypes

The file types that this document can be exported to.

**Name:** Exportable Type UTIs

## See Also

### Documents

UISupportsDocumentBrowser

A Boolean value indicating whether the app is a document-based app.

**Name:** Supports Document Browser

LSSupportsOpeningDocumentsInPlace

A Boolean value indicating whether the app may open the original document from a file provider, rather than a copy of the document.

**Name:** Supports opening documents in place

NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

