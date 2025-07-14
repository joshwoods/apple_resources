

- App Intents
- AssistantSchemas
- AssistantSchemas.IntentSchema
-  createFolder 

Instance Property

# createFolder

The app intent conforms to the schema for creating a folder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var createFolder: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.files` app intent domain, see Making file management actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.files.createFolder` schema:

```
@AssistantIntent(schema: .files.createFolder)
struct CreateFolderIntent: AppIntent {
    @Parameter
    var target: ExampleFileEntity

    @Parameter
    var fileName: String?

    func perform() async throws -> some ReturnsValue {
        let url = URL(fileURLWithPath: "some/path")
        return .result(
            value: ExampleFileEntity(id: try .file(url: url))
        )
    }
}
```

