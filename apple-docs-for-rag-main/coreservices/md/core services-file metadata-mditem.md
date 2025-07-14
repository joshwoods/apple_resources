

- Core Services
- File Metadata
-  MDItem 

API Collection

# MDItem

## Overview

MDItem is a CF-compliant object that represents a file andthe metadata associated with the file.

For functions that expect an MDItemRef parameter, if thisparameter is not a valid MDItemRef, the behavior is undefined. `NULL` isnot a valid MDItemRef.

## Topics

### Creating an MDItem

func MDItemCreate(CFAllocator!, CFString!) -> MDItem!

Creates an MDItem object for a file at the specified path.

func MDItemCreateWithURL(CFAllocator!, CFURL!) -> MDItem!

Creates an MDItem object for a file at the specified file URL.

### Getting the Type Identifier

func MDItemGetTypeID() -> CFTypeID

Returns the type identifier of all MDItem instances.

### Retrieving Metadata Attributes 

func MDItemCopyAttribute(MDItem!, CFString!) -> CFTypeRef!

Returns the value of the specified attribute in the metadata item.

func MDItemCopyAttributes(MDItem!, CFArray!) -> CFDictionary!

Returns the values of the specified attributes in the metadata item.

func MDItemCopyAttributeNames(MDItem!) -> CFArray!

Returns an array containing the attribute names existing in the metadata item.

### Data Types

class MDItem

A reference to a MDItem object.

### Constants

Common Metadata Attribute Keys

Metadata attribute keys that are common to many file types.

Image Metadata Attribute Keys

Metadata attribute keys that are common to image files.

Video Metadata Attribute Keys

Metadata attribute keys that are common to video files.

Audio Metadata Attribute Keys

Metadata attribute keys that describe an audio file.

File System Metadata Attribute Keys

Metadata attribute keys that describe the file system attributes for a file.

## See Also

### Opaque Types

MDSchema

### Related Documentation

Spotlight Overview

File Metadata Search Programming Guide

Spotlight Importer Programming Guide

File Metadata Attributes Reference

