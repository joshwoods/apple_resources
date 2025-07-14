

- CarPlay
- CPMapTemplate
-  showPanningInterface(animated:) 

Instance Method

# showPanningInterface(animated:)

Shows the panning interface on the map.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func showPanningInterface(animated: Bool)
```

## Parameters 

`animated`  

A Boolean value that determines whether to animate the panning interface.

## Discussion

Calling this method while displaying the panning interface has no effect.

While showing the panning interface, the system hides all map buttons. The system doesn’t provide a button to dismiss the panning interface. Instead, you must provide a map button in the navigation bar that the user taps to dismiss the panning interface.

## See Also

### Panning the Map

func dismissPanningInterface(animated: Bool)

Dismisses the panning interface.

var isPanningInterfaceVisible: Bool

A Boolean value that indicates whether the map template is displaying the panning interface.

