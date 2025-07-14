

- MusicKit
- ArtworkImage
-  onCommand(\_:perform:) 

Instance Method

# onCommand(\_:perform:)

Adds an action to perform in response to the given selector.

MusicKitSwiftUImacOS 10.15+

``` source
nonisolated
func onCommand(
    _ selector: Selector,
    perform action: (() -> Void)?
) -> some View
```

## Parameters 

`selector`  

The selector to register for `action`.

`action`  

The action to perform. If `action` is `nil`, `command` keeps its association with this view but doesn’t trigger.

## Return Value

A view that triggers `action` when the `command` occurs.

## Discussion

This view or one of the views it contains must be in focus in order for the action to trigger. Other actions for the same command on views *closer* to the view in focus take priority, potentially overriding this action.

