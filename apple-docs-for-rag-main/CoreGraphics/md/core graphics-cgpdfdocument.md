

- Core Graphics
-  CGPDFDocument 

Class

# CGPDFDocument

A document that contains PDF (Portable Document Format) drawing information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGPDFDocument
```

## Overview

PDF provides an efficient format for cross-platform exchange of documents with rich content. PDF files can contain multiple pages of images and text. A PDF document object contains all the information relating to a PDF document, including its catalog and contents.

Note that PDF documents may be encrypted, and that some operations may be restricted until a valid password is supplied—see the functions listed in Working with an Encrypted PDF Document. Core Graphics also supports decrypting encrypted documents.

Core Graphics can both display and generate files that are compliant with the PDF standard.

## Topics

### Creating PDF Documents

init?(CGDataProvider)

Creates a Core Graphics PDF document using a data provider.

init?(CFURL)

Creates a Core Graphics PDF document using data specified by a URL.

### Examining a PDF Document

var catalog: CGPDFDictionaryRef?

Returns the document catalog of a Core Graphics PDF document.

var fileIdentifier: CGPDFArrayRef?

Gets the file identifier for a PDF document.

var info: CGPDFDictionaryRef?

Gets the information dictionary for a PDF document.

var numberOfPages: Int

Returns the number of pages in a PDF document.

func getVersion(majorVersion: UnsafeMutablePointer&lt;Int32>, minorVersion: UnsafeMutablePointer&lt;Int32>)

Returns the major and minor version numbers of a Core Graphics PDF document.

func page(at: Int) -> CGPDFPage?

Returns a page from a Core Graphics PDF document.

### Working with an Encrypted PDF Document

var isEncrypted: Bool

Returns whether the specified PDF file is encrypted.

var allowsCopying: Bool

Returns whether the specified PDF document allows copying.

var allowsPrinting: Bool

Returns whether a PDF document allows printing.

var isUnlocked: Bool

Returns whether the specified PDF document is currently unlocked.

func unlockWithPassword(UnsafePointer&lt;CChar>) -> Bool

Unlocks an encrypted PDF document when a valid password is supplied.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the type identifier for Core Graphics PDF documents.

### Abstract Types for PDF Document Content

Use these abstract types and related functions to work with the content of a CGPDFDocument object.

class CGPDFPage

A type that represents a page in a PDF document.

CGPDFArray

An array structure within a PDF document.

CGPDFObject

An object representing content within a PDF document.

CGPDFStream

A stream or sequence of data bytes in a PDF document.

CGPDFString

A text string in a PDF document.

CGPDFScanner

A parser object for handling content and operators in a PDF content stream.

CGPDFDictionary

A dictionary structure within a PDF document.

CGPDFContentStream

A representation of one or more content data streams in a PDF page.

CGPDFOperatorTable

A set of callback functions for operators used when scanning content in a PDF document.

### Instance Properties

var accessPermissions: CGPDFAccessPermissions

var outline: CFDictionary?

## Relationships

### Conforms To

- Equatable
- Hashable

