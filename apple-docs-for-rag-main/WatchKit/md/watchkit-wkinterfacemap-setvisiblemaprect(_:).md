

- WatchKit
- WKInterfaceMap
-  setVisibleMapRect(\_:) 

Instance Method

# setVisibleMapRect(\_:)

Changes the map’s visible region to the specified map rectangle.

watchOS 2.0+

``` source
func setVisibleMapRect(_ mapRect: MKMapRect)
```

## Parameters 

`mapRect`  

The region to be displayed, specified as a map rectangle. The size of the rectangle provides an implicit zoom value for the map. For more information about the MKMapRect type, see MapKit.

## Discussion

The method may adjust the specified map rectangle slightly to fit the available display space for the map. The adjusted region always includes the entire region you specified.

Changing the visible region may require the loading of additional map tiles to render the map. Loading tiles requires an active network connection.

## See Also

### Related Documentation

App Programming Guide for watchOS

### Specifying the Map Region

func setRegion(MKCoordinateRegion)

Changes the map’s visible region to the specified coordinate region.

