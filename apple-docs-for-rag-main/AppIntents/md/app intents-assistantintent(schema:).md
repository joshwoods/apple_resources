

- App Intents
-  AssistantIntent(schema:) 

Macro

# AssistantIntent(schema:)

A Swift macro you use to make sure your app intent conforms to an assistant schema.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@attached(memberAttribute) @attached(extension, conformances: AssistantSchemaIntent, ShowInAppSearchResultsIntent, names: named(__assistantSchemaIntent)) macro AssistantIntent(schema: T) where T : AssistantSchemas.Intent
```

## Mentioned in 

Making email actions available to Siri and Apple Intelligence

Making file management actions available to Siri and Apple Intelligence

Making photo and video actions available to Siri and Apple Intelligence

Making spreadsheet actions available to Siri and Apple Intelligence

Making presentation actions available to Siri and Apple Intelligence

## See Also

### Macros

macro AssistantEntity&lt;T>(schema: T)

A Swift macro you use to make sure your app entity conforms to an assistant schema.

macro AssistantEnum&lt;T>(schema: T)

A Swift macro you use to make sure your app enum conforms to an assistant schema.

