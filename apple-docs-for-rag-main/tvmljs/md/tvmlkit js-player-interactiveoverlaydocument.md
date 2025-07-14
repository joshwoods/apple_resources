

- TVMLKit JS
- Player
-  interactiveOverlayDocument 

Instance Property

# interactiveOverlayDocument

A DOM document that is presented over the entire video player, including the transport bar.

tvOS 10.0+

``` source
attribute Document interactiveOverlayDocument;
```

## Discussion

The interactive overlay document can contain focusable elements and can be any template document. Set this attribute to `null` to remove the current overlay document.

## See Also

### Setting Up the Player

interactiveOverlayDismissable

Determines if an interactive overlay can be dismissed using the Menu button.

overlayDocument

The annotations for a video created by placing a DOM document over the video.

Player

Creates a new player object.

playlist

The playlist for a player.

present

Shows the player UI if it is not currently visible.

