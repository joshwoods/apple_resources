

- App Intents
- EntityProperty
-  init(title:) 

Initializer

# init(title:)

Creates an app intent entity property.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
convenience init(title: LocalizedStringResource)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `Measurement`.

## Parameters 

`title`  

A word or short phrase summarizing this property.

