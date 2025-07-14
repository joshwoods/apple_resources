

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  updateSheet 

Instance Property

# updateSheet

The app intent conforms to the schema for updating a sheet in a spreadsheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var updateSheet: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.spreadsheet` app intent domain, see Making spreadsheet actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.spreadsheet.updateSheet` schema:

```
@AssistantIntent(schema: .spreadsheet.updateSheet)
struct UpdateSheetIntent: AppIntent {
    @Parameter
    var target: SheetEntity

    @Parameter
    var name: String?

    @Parameter
    var position: Int?

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

