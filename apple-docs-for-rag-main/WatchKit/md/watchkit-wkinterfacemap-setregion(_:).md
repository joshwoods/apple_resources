

- WatchKit
- WKInterfaceMap
-  setRegion(\_:) 

Instance Method

# setRegion(\_:)

Changes the map’s visible region to the specified coordinate region.

watchOS 2.0+

``` source
func setRegion(_ coordinateRegion: MKCoordinateRegion)
```

## Parameters 

`coordinateRegion`  

The new region of the map to be displayed. The span value of this parameter provides an implicit zoom value for the map. For more information about the MKCoordinateRegion type, see MapKit.

## Discussion

This method changes the currently visible region of the map. The method may adjust the map rectangle slightly to fit the available display space for the map. The adjusted region always includes the entire region you specified.

Changing the visible region may require the loading of additional map tiles to render the map. Loading tiles requires an active network connection.

## See Also

### Specifying the Map Region

func setVisibleMapRect(MKMapRect)

Changes the map’s visible region to the specified map rectangle.

