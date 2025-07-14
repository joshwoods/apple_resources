

- App Intents
-  FileEntityIdentifier 

Structure

# FileEntityIdentifier

An identifier for an app entity that refers to a document or other file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct FileEntityIdentifier
```

## Topics

### Operators

static func == (FileEntityIdentifier, FileEntityIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var draftIdentifier: String?

The document draft identifier, if the document hasn’t been materialized on disk yet.

var fileURL: URL?

A URL that locates a file saved to disk.

var hashValue: Int

The hash value.

var isDraft: Bool

Indicates whether this identifier represents a document draft.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Methods

static func draft(identifier: String) -> FileEntityIdentifier

Creates and returns an identifier for a draft document.

static func file(url: URL) throws -> FileEntityIdentifier

Creates and returns an identifier with the provided URL to the file on disk.

### Default Implementations

EntityIdentifierConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- EntityIdentifierConvertible
- Equatable
- Hashable
- Sendable

