

- CarPlay
- CPNowPlayingButton
-  isSelected 

Instance Property

# isSelected

A Boolean value that indicates whether the button is in a selected state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isSelected: Bool { get set }
```

## Discussion

When this property is set to true, CarPlay draws the button with a selected appearance to indicate its selected state. You can only update this property manually on instances of CPNowPlayingImageButton. All system-provided buttons—for example, CPNowPlayingShuffleButton or CPNowPlayingRepeatButton—manage their own selected states internally.

The default value is false.

## See Also

### Managing the Button State

var isEnabled: Bool

A Boolean value that indicates whether the button is in an enabled state.

