

- AVKit
- AVNavigationMarkersGroup
-  dateRangeNavigationMarkers 

Instance Property

# dateRangeNavigationMarkers

The array of date range navigation markers for which the group provides navigation.

tvOS 9.0+

``` source
var dateRangeNavigationMarkers: [AVDateRangeMetadataGroup]? { get }
```

## Discussion

Returns the array of AVDateRangeMetadataGroup objects managed by this group. This value may be `nil`.

## See Also

### Inspecting Navigation Metadata

var title: String?

The title of the marker group.

var timedNavigationMarkers: [AVTimedMetadataGroup]?

The array of timed navigation markers for which the group provides navigation.

