

- App Intents
- IntentItemCollection
-  init(promptLabel:usesIndexedCollation:items:) 

Initializer

# init(promptLabel:usesIndexedCollation:items:)

Create a `ItemCollection` containing `Items`, or one or more `Sections`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    promptLabel: LocalizedStringResource? = nil,
    usesIndexedCollation: Bool = false,
    items: [Result]
) where Result : DisplayRepresentable
```

