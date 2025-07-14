

- CarPlay
- CPMapTemplate
-  dismissPanningInterface(animated:) 

Instance Method

# dismissPanningInterface(animated:)

Dismisses the panning interface.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func dismissPanningInterface(animated: Bool)
```

## Parameters 

`animated`  

A Boolean value that determines whether to animate the dismissal of the panning interface. Set to true to animate the dismissal.

## Discussion

When dismissing the panning interface, the system shows the previously hidden map buttons.

## See Also

### Panning the Map

func showPanningInterface(animated: Bool)

Shows the panning interface on the map.

var isPanningInterfaceVisible: Bool

A Boolean value that indicates whether the map template is displaying the panning interface.

