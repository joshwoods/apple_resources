

- App Intents
- AppShortcutParameterPresentation
-  init(for:summary:optionsCollections:) 

Initializer

# init(for:summary:optionsCollections:)

Creates an object that represents the App Shortcut with the specified parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    for keyPath: ParameterKeyPath,
    summary: AppShortcutParameterPresentationSummary,
    @AppShortcutOptionsCollectionSpecificationBuilder optionsCollections: () -> some AppShortcutOptionsCollectionSpecification
)
```

## Parameters 

`summary`  

Represents the summary of the parameter used in the presentation.

