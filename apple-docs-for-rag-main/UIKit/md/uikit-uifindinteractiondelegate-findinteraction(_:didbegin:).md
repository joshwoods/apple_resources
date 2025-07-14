

- UIKit
- UIFindInteractionDelegate
-  findInteraction(\_:didBegin:) 

Instance Method

# findInteraction(\_:didBegin:)

Informs the delegate when the interaction is about to present the find panel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func findInteraction(
    _ interaction: UIFindInteraction,
    didBegin session: UIFindSession
)
```

## Parameters 

`interaction`  

The interaction object triggering the find panel.

`session`  

The session object you provided for the interaction.

## Discussion

Use this method to decorate your view to indicate that a search operation is about to occur. For example, apply a dimming view around the unhighlighted search results.

## See Also

### Decorating the searched content

func findInteraction(UIFindInteraction, didEnd: UIFindSession)

Informs the delegate when the interaction is about to dismiss the find panel.

