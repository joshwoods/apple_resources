

- App Intents
- SiriTipView
-  writingToolsAffordanceVisibility(\_:) 

Instance Method

# writingToolsAffordanceVisibility(\_:)

Specifies whether the system should show the Writing Tools affordance for text input views affected by the environment.

AppIntentsSwiftUIiOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
@MainActor @preconcurrency
func writingToolsAffordanceVisibility(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

Whether the affordance may be shown for text input views.

## Discussion

Use this view modifier to disable the Writing Tools affordance for `TextField` views when running on macOS or Mac Catalyst.

Parameters:

Returns: A view with the specified Writing Tools affordance visibility.

