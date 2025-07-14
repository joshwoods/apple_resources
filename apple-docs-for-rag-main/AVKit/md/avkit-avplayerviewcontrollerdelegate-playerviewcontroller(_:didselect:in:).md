

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:didSelect:in:) 

Instance Method

# playerViewController(\_:didSelect:in:)

Tells the delegate when the user selects a media option from a media selection group.

tvOS 9.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    didSelect mediaSelectionOption: AVMediaSelectionOption?,
    in mediaSelectionGroup: AVMediaSelectionGroup
)
```

## Parameters 

`playerViewController`  

The player view controller.

`mediaSelectionOption`  

The user’s selected media option, which may be `nil`.

`mediaSelectionGroup`  

The media selection group in which the selected media option exists.

