

- Authentication Services
- ASImportableCredential
-  ASImportableCredential.Note 

Structure

# ASImportableCredential.Note

A piece of text used to store some information about an item.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct Note
```

## Topics

### Creating a note

init(content: String)

Creates a note instance from the note contents.

### Accessing note properties

var content: String

The contents of the note.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Document credential types

case note(ASImportableCredential.Note)

A note credential.

