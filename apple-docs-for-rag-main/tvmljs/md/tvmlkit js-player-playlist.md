

- TVMLKit JS
- Player
-  playlist 

Instance Property

# playlist

The playlist for a player.

tvOS 9.0+

``` source
attribute Playlist playlist;
```

## Discussion

Setting this attribute changes the Playlist object associated with the player. Inspect this attribute to get the Playlist object currently associated with the player.

## See Also

### Setting Up the Player

interactiveOverlayDismissable

Determines if an interactive overlay can be dismissed using the Menu button.

interactiveOverlayDocument

A DOM document that is presented over the entire video player, including the transport bar.

overlayDocument

The annotations for a video created by placing a DOM document over the video.

Player

Creates a new player object.

present

Shows the player UI if it is not currently visible.

