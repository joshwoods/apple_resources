

- TVMLKit JS
- Player
-  overlayDocument 

Instance Property

# overlayDocument

The annotations for a video created by placing a DOM document over the video.

tvOS 9.0+

``` source
attribute Document overlayDocument;
```

## Discussion

Create a DOM document using the divTemplate and assign it to the `overlayDocument` property. Set this attribute to `null` to remove the current overlay document.

## See Also

### Setting Up the Player

interactiveOverlayDismissable

Determines if an interactive overlay can be dismissed using the Menu button.

interactiveOverlayDocument

A DOM document that is presented over the entire video player, including the transport bar.

Player

Creates a new player object.

playlist

The playlist for a player.

present

Shows the player UI if it is not currently visible.

