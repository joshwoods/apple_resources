

- Core Graphics
- CGContext
-  Auxiliary Dictionary Keys 

API Collection

# Auxiliary Dictionary Keys

Keys for the auxiliary info dictionary you specify when creating a PDF context.

## Overview

For more information about using these keys in a PDF context, see init(consumer:mediaBox:_:) and init(_:mediaBox:_:).

## Topics

### Metadata Keys

let kCGPDFContextAuthor: CFString

The corresponding value is a string that represents the name of the person who created the document. This key is optional.

let kCGPDFContextCreator: CFString

The corresponding value is a string that represents the name of the application used to produce the document. This key is optional.

let kCGPDFContextTitle: CFString

The corresponding value is a string that represents the title of the document. This key is optional.

let kCGPDFContextOwnerPassword: CFString

let kCGPDFContextUserPassword: CFString

let kCGPDFContextAllowsPrinting: CFString

Whether the document allows printing when unlocked with the user password.

let kCGPDFContextAllowsCopying: CFString

Whether the document allows copying when unlocked with the user password.

let kCGPDFContextOutputIntent: CFString

let kCGPDFContextOutputIntents: CFString

let kCGPDFContextSubject: CFString

let kCGPDFContextKeywords: CFString

let kCGPDFContextEncryptionKeyLength: CFString

### Box Keys

let kCGPDFContextMediaBox: CFString

The media box for the document or for a given page.

let kCGPDFContextCropBox: CFString

The crop box for the document or for a given page.

let kCGPDFContextBleedBox: CFString

The bleed box for the document or for a given page.

let kCGPDFContextTrimBox: CFString

The trim box for the document or for a given page.

let kCGPDFContextArtBox: CFString

The art box for the document or for a given page.

### Output Intent Keys

let kCGPDFXOutputIntentSubtype: CFString

The output intent subtype. This key is required.

let kCGPDFXOutputConditionIdentifier: CFString

let kCGPDFXOutputCondition: CFString

A text string identifying the intended output device or production condition in a human-readable form.

let kCGPDFXRegistryName: CFString

let kCGPDFXInfo: CFString

let kCGPDFXDestinationOutputProfile: CFString

## See Also

### Creating PDF Graphics Contexts

init?(CFURL, mediaBox: UnsafePointer&lt;CGRect>?, CFDictionary?)

Creates a URL-based PDF graphics context.

init?(consumer: CGDataConsumer, mediaBox: UnsafePointer&lt;CGRect>?, CFDictionary?)

Creates a PDF graphics context.

