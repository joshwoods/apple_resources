

- App Intents
- ShortcutsLink
-  accessibilityIdentifier(\_:isEnabled:) 

Instance Method

# accessibilityIdentifier(\_:isEnabled:)

Uses the string you specify to identify the view.

AppIntentsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityIdentifier(
    _ identifier: String,
    isEnabled: Bool
) -> ModifiedContent
```

## Parameters 

`identifier`  

The accessibility identifier to apply.

`isEnabled`  

If true the accessibility identifier is applied; otherwise the accessibility identifier is unchanged.

## Discussion

Use this value for testing. It isn’t visible to the user.

