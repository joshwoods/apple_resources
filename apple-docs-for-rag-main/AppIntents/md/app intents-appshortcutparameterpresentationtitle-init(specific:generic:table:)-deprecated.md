

- App Intents
- AppShortcutParameterPresentationTitle
-  init(specific:generic:table:) Deprecated

Initializer

# init(specific:generic:table:)

Initializes an `AppShortcutParameterPresentationTitle` with the specified parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+tvOS 17.0+

``` source
init(
    specific: AppShortcutParameterPresentationTitleString,
    generic: StaticString,
    table: StaticString? = nil
)
```

Deprecated

Please use init(for:summary:optionsCollections:)

## Parameters 

`specific`  

An `AppShortcutParameterPresentationTitleString` representing the specific title of the `AppShortcutParameterPresentation`. Example: `"Call \(\.$person)"`.

`generic`  

A `StaticString` representing the generic title of the `AppShortcutParameterPresentation`. Example: `"Call Person..."`.

`table`  

An optional `StaticString` representing the table to use when localizing the title.

