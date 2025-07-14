

- AVKit
- AVNavigationMarkersGroup
-  title 

Instance Property

# title

The title of the marker group.

tvOS 9.0+

``` source
var title: String? { get }
```

## Discussion

You set a marker group’s title with the AVNavigationMarkersGroup initializer. Each marker group in the navigationMarkerGroups array of an AVPlayerItem object must have a unique title. To use the marker group as a chapter list, set its title to `nil`.

## See Also

### Inspecting Navigation Metadata

var timedNavigationMarkers: [AVTimedMetadataGroup]?

The array of timed navigation markers for which the group provides navigation.

var dateRangeNavigationMarkers: [AVDateRangeMetadataGroup]?

The array of date range navigation markers for which the group provides navigation.

