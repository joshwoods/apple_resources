

- SwiftUI
-  ReferenceFileDocumentConfiguration 

Structure

# ReferenceFileDocumentConfiguration

The properties of an open reference file document.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct ReferenceFileDocumentConfiguration where Document : ReferenceFileDocument
```

## Overview

You receive an instance of this structure when you create a DocumentGroup with a reference file type. Use it to access the document in your viewer or editor.

## Topics

### Getting and setting the document

var document: Document

The current document model.

var $document: ObservedObject&lt;Document>.Wrapper

### Getting document properties

var fileURL: URL?

The URL of the open file document.

var isEditable: Bool

A Boolean that indicates whether you can edit the document.

## See Also

### Storing document data in a class instance

protocol ReferenceFileDocument

A type that you use to serialize reference type documents to and from file.

var undoManager: UndoManager?

The undo manager used to register a view’s undo operations.

