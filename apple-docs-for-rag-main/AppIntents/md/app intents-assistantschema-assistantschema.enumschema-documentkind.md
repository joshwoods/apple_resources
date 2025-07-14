

- App Intents
- AssistantSchema
- AssistantSchema.EnumSchema
-  documentKind 

Instance Property

# documentKind

The file type for a document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var documentKind: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.reader` app intent domain, see Making document reader actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.reader.documentKind` schema:

```
@AssistantEnum(schema: .reader.documentKind)
enum ReaderDocumentKind: AppEnum, Codable {
    case image
    case pdf

    static var caseDisplayRepresentations: [Self: DisplayRepresentation] {
        [
            .image: .init(title: "Image", image: .init(systemName: "photo")),
            .pdf: .init(title: "PDF", image: .init(systemName: "doc.text")),
        ]
    }
}
```

