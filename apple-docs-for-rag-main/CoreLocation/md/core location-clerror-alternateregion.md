

- Core Location
- CLError
-  alternateRegion 

Instance Property

# alternateRegion

A region that location services can monitor more effectively.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+

``` source
var alternateRegion: CLRegion? { get }
```

## Discussion

This property has a value only for errors of type regionMonitoringResponseDelayed.

