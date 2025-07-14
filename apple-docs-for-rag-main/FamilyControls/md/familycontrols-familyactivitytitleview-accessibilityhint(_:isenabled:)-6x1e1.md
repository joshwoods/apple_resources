

- FamilyControls
- FamilyActivityTitleView
-  accessibilityHint(\_:isEnabled:) 

Instance Method

# accessibilityHint(\_:isEnabled:)

Communicates to the user what happens after performing the view’s action.

FamilyControlsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityHint(
    _ hintKey: LocalizedStringKey,
    isEnabled: Bool
) -> ModifiedContent
```

## Parameters 

`hintKey`  

The accessibility hint to apply.

`isEnabled`  

If true the accessibility hint is applied; otherwise the accessibility hint is unchanged.

## Discussion

Provide a hint in the form of a brief phrase, like “Purchases the item” or “Downloads the attachment”.

