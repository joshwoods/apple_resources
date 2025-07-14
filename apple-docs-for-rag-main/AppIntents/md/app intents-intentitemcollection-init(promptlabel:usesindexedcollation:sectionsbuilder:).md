

- App Intents
- IntentItemCollection
-  init(promptLabel:usesIndexedCollation:sectionsBuilder:) 

Initializer

# init(promptLabel:usesIndexedCollation:sectionsBuilder:)

Create an `ItemCollection` containing `Items`, or one or more `Sections` provided by a builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    promptLabel: LocalizedStringResource? = nil,
    usesIndexedCollation: Bool = false,
    @IntentItemSection.Builder sectionsBuilder: () -> [IntentItemSection]
)
```

