

- Cinematic
- CNScript
-  removeUserDecision(\_:) 

Instance Method

# removeUserDecision(\_:)

Removes an existing user decision.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func removeUserDecision(_ decision: CNDecision) -> Bool
```

## Parameters 

`decision`  

The user decision added to the script or one made at recording time by tapping on the script.

## Return Value

A flag indicating whether the user decisions was removed.

## Discussion

You can’t remove decisions that aren’t user decisions.

