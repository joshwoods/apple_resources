

- SwiftUI
-  FileDocumentConfiguration 

Structure

# FileDocumentConfiguration

The properties of an open file document.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct FileDocumentConfiguration where Document : FileDocument
```

## Overview

You receive an instance of this structure when you create a DocumentGroup with a value file type. Use it to access the document in your viewer or editor.

## Topics

### Getting and setting the document

var document: Document

The current document model.

var $document: Binding&lt;Document>

### Getting document properties

var fileURL: URL?

The URL of the open file document.

var isEditable: Bool

A Boolean that indicates whether you can edit the document.

## See Also

### Storing document data in a structure instance

protocol FileDocument

A type that you use to serialize documents to and from file.

