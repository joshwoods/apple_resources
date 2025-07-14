

- App Intents
- EntityProperty
-  init(title:) 

Initializer

# init(title:)

Creates an app intent entity property.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(title: LocalizedStringResource)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` conforms to `AppEntity`.

## Parameters 

`title`  

A word or short phrase summarizing this property.

