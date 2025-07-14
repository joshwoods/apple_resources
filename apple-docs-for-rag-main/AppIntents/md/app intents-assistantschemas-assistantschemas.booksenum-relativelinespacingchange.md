

- App Intents
- AssistantSchemas
- AssistantSchemas.BooksEnum
-  relativeLineSpacingChange 

Instance Property

# relativeLineSpacingChange

The relative change in line spacing for rendering a book.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var relativeLineSpacingChange: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.books` app intent domain, see Making ebook actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.books.relativeLineSpacingChange` schema:

```
@AssistantEnum(schema: .books.relativeLineSpacingChange)
enum BookRelativeLineSpacingChange: AppEnum {
    case `default`

    static var caseDisplayRepresentations: [BookRelativeLineSpacingChange: AppIntents.DisplayRepresentation] = [
        .`default`: "Default"
    ]
}
```

