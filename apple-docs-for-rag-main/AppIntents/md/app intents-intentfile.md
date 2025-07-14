

- App Intents
-  IntentFile 

Structure

# IntentFile

An interface for providing an app entity that represents an on-disk file or file-based resource.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentFile
```

## Mentioned in 

Adding parameters to an app intent

## Overview

Provide an intent file entity implementation to describe data you store in a file on disk or in memory by providing its associated name and uniform type identifier.

## Topics

### Creating a file

init(data: Data, filename: String, type: UTType?)

init(fileURL: URL, filename: String?, type: UTType?)

### Getting the file information

var filename: String

The human-readable name of the file, which will be displayed to the user.

var fileURL: URL?

URL to the file on disk, if any. If the file isn’t stored on disk, access the contents using the `data` property.

var type: UTType?

The uniform type identifier of the file. (i.e. “public.json”, “public.png”, or any custom type) More information about uniform type identifiers can be found in \

var data: Data

The contents of the file. If the file was created with a URL, accessing this property will memory map the file contents.

var removedOnCompletion: Bool

Indicates whether the file should be automatically deleted from disk when the Shortcut is done running. `false` by default.

### Instance Properties

var availableContentTypes: [UTType]

Valid content types the `IntentFile` can possibly be converted to.

### Instance Methods

func data(contentType: UTType) async throws -> Data

Requests an `IntentFile` representation as binary data of the requested content type if possible.

func file(contentType: UTType, destinationDirectory: URL?) async throws -> (fileURL: URL, openedInPlace: Bool)

Requests an `IntentFile` representation as a file url.

func withFile&lt;Result>(contentType: UTType, allowOpenInPlace: Bool, fileHandler: (URL, Bool) async throws -> Result) async throws -> Result

Requests an `IntentFile` representation as a file url.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;IntentFile>

### Enumerations

enum IntentFileError

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

InstanceDisplayRepresentable Implementations

TypeDisplayRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- Decodable
- DisplayRepresentable
- Encodable
- Equatable
- Hashable
- InstanceDisplayRepresentable
- Sendable
- TypeDisplayRepresentable

