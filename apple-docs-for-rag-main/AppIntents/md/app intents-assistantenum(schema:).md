

- App Intents
-  AssistantEnum(schema:) 

Macro

# AssistantEnum(schema:)

A Swift macro you use to make sure your app enum conforms to an assistant schema.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@attached(extension, conformances: AssistantSchemaEnum, names: named(__assistantSchemaEnum)) macro AssistantEnum(schema: T) where T : AssistantSchemas.Enum
```

## Mentioned in 

Integrating actions with Siri and Apple Intelligence

Making photo and video actions available to Siri and Apple Intelligence

Making whiteboard actions available to Siri and Apple Intelligence

Making document reader actions available to Siri and Apple Intelligence

Making browser actions available to Siri and Apple Intelligence

## See Also

### Macros

macro AssistantIntent&lt;T>(schema: T)

A Swift macro you use to make sure your app intent conforms to an assistant schema.

macro AssistantEntity&lt;T>(schema: T)

A Swift macro you use to make sure your app entity conforms to an assistant schema.

