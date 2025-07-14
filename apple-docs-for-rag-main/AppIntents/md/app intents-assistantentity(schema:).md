

- App Intents
-  AssistantEntity(schema:) 

Macro

# AssistantEntity(schema:)

A Swift macro you use to make sure your app entity conforms to an assistant schema.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@attached(memberAttribute) @attached(extension, conformances: AppEntity, AssistantSchemaEntity, names: named(__assistantSchemaEntity)) macro AssistantEntity(schema: T) where T : AssistantSchemas.Entity
```

## Mentioned in 

Making browser actions available to Siri and Apple Intelligence

Making file management actions available to Siri and Apple Intelligence

Making email actions available to Siri and Apple Intelligence

Making document reader actions available to Siri and Apple Intelligence

Making word processor actions available to Siri and Apple Intelligence

## See Also

### Macros

macro AssistantIntent&lt;T>(schema: T)

A Swift macro you use to make sure your app intent conforms to an assistant schema.

macro AssistantEnum&lt;T>(schema: T)

A Swift macro you use to make sure your app enum conforms to an assistant schema.

