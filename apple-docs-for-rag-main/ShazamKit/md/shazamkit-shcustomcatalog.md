

- ShazamKit
-  SHCustomCatalog 

Class

# SHCustomCatalog

An object for storing the reference signatures for custom audio recordings and their associated metadata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHCustomCatalog
```

## Overview

Create a custom catalog by adding reference signatures that you generate from audio that you provide. You also add the associated metadata for each signature. Save your custom catalog and share it with others. You can also load a saved catalog.

## Topics

### Creating a custom catalog object

init()

Creates a new custom catalog object for storing reference audio signatures and their associated metadata.

### Adding a signature to the catalog

func addReferenceSignature(SHSignature, representing: [SHMediaItem]) throws

Adds a reference signature and its associated metadata to a catalog.

### Loading and saving a custom catalog

func add(from: URL) throws

Loads a saved custom catalog from a file.

func write(to: URL) throws

Saves the custom catalog to a local file.

Deprecated

### Getting the content type

static var shazamCustomCatalog: UTType { get }

A type that represents a custom catalog.

### Initializers

init(dataRepresentation: Data) throws

Load a @c SHCustomCatalog from data

### Instance Properties

var dataRepresentation: Data

The data representation of this file, it can be written to disk

## Relationships

### Inherits From

- SHCatalog

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Create a custom audio catalog

Building a Custom Catalog and Matching Audio

Display lesson content that’s synchronized to a learning video by matching the audio to a custom reference signature and associated metadata.

ShazamKit Dance Finder with Managed Session

Find a video of dance moves for a specific song by matching the audio to a custom catalog, and show a history of recognized songs.

class SHCatalog

An abstract base class for storing reference signatures and their associated metadata.

