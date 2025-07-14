

- App Intents
- AppShortcutParameterPresentationSummary
-  init(\_:table:) 

Initializer

# init(\_:table:)

Initializes a presentation summary with the specified parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ summaryString: AppShortcutParameterPresentationSummaryString,
    table: StaticString? = nil
)
```

## Parameters 

`summaryString`  

Represents the summary of the AppShortcutParameterPresentation. Example: “Call (.\$person)”.

`table`  

An optional `StaticString` representing the table to use when localizing the summary.

