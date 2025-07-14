

- AVKit
- AVNavigationMarkersGroup
-  timedNavigationMarkers 

Instance Property

# timedNavigationMarkers

The array of timed navigation markers for which the group provides navigation.

tvOS 9.0+

``` source
var timedNavigationMarkers: [AVTimedMetadataGroup]? { get }
```

## Discussion

Returns the array of AVTimedMetadataGroup objects managed by this group. This value may be `nil`.

## See Also

### Inspecting Navigation Metadata

var title: String?

The title of the marker group.

var dateRangeNavigationMarkers: [AVDateRangeMetadataGroup]?

The array of date range navigation markers for which the group provides navigation.

