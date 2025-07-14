

- Bundle Resources
- Information Property List
-  NSDownloadsUbiquitousContents 

Property List Key

# NSDownloadsUbiquitousContents

A Boolean value that indicates whether the system should download documents before handing them over to the app.

macOS 11.0+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

By default, the system displays the download progress. Set the value to `YES` if you want your app to display a custom download progress indicator instead.

## See Also

### Documents

CFBundleDocumentTypes

The document types supported by the bundle.

**Name:** Document types

UISupportsDocumentBrowser

A Boolean value indicating whether the app is a document-based app.

**Name:** Supports Document Browser

LSSupportsOpeningDocumentsInPlace

A Boolean value indicating whether the app may open the original document from a file provider, rather than a copy of the document.

**Name:** Supports opening documents in place

