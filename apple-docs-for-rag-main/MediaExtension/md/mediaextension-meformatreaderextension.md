

- MediaExtension
-  MEFormatReaderExtension 

Protocol

# MEFormatReaderExtension

A protocol that defines a factory to create a new format reader with a byte source.

macOS 14.0+

``` source
protocol MEFormatReaderExtension : NSObjectProtocol
```

## Overview

Media Toolbox creates the `MEFormatReaderExtension` object and the MEByteSource object based on the media asset.

## Topics

### Creating a format reader

init()

Creates a new format reader factory.

**Required**

func formatReader(with: MEByteSource, options: MEFormatReaderInstantiationOptions?) throws -> any MEFormatReader

Creates a new format reader with the byte source and options that you specify.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Format readers

protocol MEFormatReader

A protocol that defines the requirements for a format reader, which represents a single media asset.

class MEFormatReaderInstantiationOptions

An object that contains options to pass to a format reader extension.

class MEFileInfo

An object that contains file properties from the media asset.

Format reader property list dictionaries

Include property list dictionaries to describe a format reader and register the formats it supports.

Format reader entitlement

Include an entitlement to indicate your extension is a MediaExtension format reader.

