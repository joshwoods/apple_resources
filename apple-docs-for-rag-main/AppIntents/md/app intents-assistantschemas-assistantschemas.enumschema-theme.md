

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  theme 

Instance Property

# theme

The theme for rendering a book.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var theme: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.books` app intent domain, see Making ebook actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.books.theme` schema:

```
@AssistantEnum(schema: .books.theme)
enum BookTheme: AppEnum {
    case lightMode
    case darkMode
    case theme1

    static var caseDisplayRepresentations: [BookTheme: AppIntents.DisplayRepresentation] = [
        .lightMode: "Light Mode",
        .darkMode: "Dark Mode",
        .theme1: "Theme 1",
    ]
}
```

