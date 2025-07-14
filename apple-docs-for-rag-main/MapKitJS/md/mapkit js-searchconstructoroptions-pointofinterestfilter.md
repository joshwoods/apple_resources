

- MapKit JS
- SearchConstructorOptions
-  pointOfInterestFilter 

Instance Property

# pointOfInterestFilter

A filter used to include or exclude point of interest categories.

MapKit JS 5.32.2+

``` source
attribute mapkit.PointOfInterestFilter pointOfInterestFilter;
```

## Discussion

If you provide a mapkit.PointOfInterestFilter and set includePointsOfInterest to `false`, the filter takes precedence and MapKit JS ignores the Boolean.

## See Also

### Points of Interest

includePointsOfInterest

A Boolean value that indicates whether the search results should include points of interest.

