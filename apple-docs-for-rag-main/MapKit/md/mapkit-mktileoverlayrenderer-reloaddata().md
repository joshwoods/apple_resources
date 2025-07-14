

- MapKit
- MKTileOverlayRenderer
-  reloadData() 

Instance Method

# reloadData()

Forces the tile overlay renderer to reload and redisplay the tiles.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
func reloadData()
```

## Discussion

Use this method to remove the overlay’s existing tile images and reload them from the original source. This method automatically causes the renderer to redraw the new tiles as soon as it loads them into memory.

