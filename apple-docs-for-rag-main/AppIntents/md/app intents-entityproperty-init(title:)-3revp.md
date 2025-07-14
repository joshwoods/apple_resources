

- App Intents
- EntityProperty
-  init(title:) 

Initializer

# init(title:)

Creates an app intent entity property.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
convenience init(title: LocalizedStringResource)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Calendar.RecurrenceRule`.

## Parameters 

`title`  

A word or short phrase summarizing this property.

