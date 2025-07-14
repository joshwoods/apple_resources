

- UIKit
- UISpringLoadedInteractionBehavior
-  interactionDidFinish(\_:) 

Instance Method

# interactionDidFinish(\_:)

Tells the behavior object when the spring-loading interaction is finished, either because it was canceled or because spring loading was activated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func interactionDidFinish(_ interaction: UISpringLoadedInteraction)
```

## Parameters 

`interaction`  

The spring-loaded interaction requesting the information.

