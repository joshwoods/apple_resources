

- UIKit
- UIFindInteractionDelegate
-  findInteraction(\_:didEnd:) 

Instance Method

# findInteraction(\_:didEnd:)

Informs the delegate when the interaction is about to dismiss the find panel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func findInteraction(
    _ interaction: UIFindInteraction,
    didEnd session: UIFindSession
)
```

## Parameters 

`interaction`  

The interaction object triggering the find panel.

`session`  

The session object you provided for the interaction.

## Discussion

Use this method to undo decoration on your view to indicate that a search operation is complete. For example, remove a dimming view from around the unhighlighted search results.

## See Also

### Decorating the searched content

func findInteraction(UIFindInteraction, didBegin: UIFindSession)

Informs the delegate when the interaction is about to present the find panel.

