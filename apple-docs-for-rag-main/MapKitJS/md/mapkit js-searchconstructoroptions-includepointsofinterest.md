

- MapKit JS
- SearchConstructorOptions
-  includePointsOfInterest 

Instance Property

# includePointsOfInterest

A Boolean value that indicates whether the search results should include points of interest.

MapKit JS 5.32.2+

``` source
attribute boolean includePointsOfInterest;
```

## Discussion

If you set this value to `false` and include a pointOfInterestFilter, the filter takes precedence and MapKit JS ignores the `false` value. The default value is `true`.

## See Also

### Points of Interest

pointOfInterestFilter

A filter used to include or exclude point of interest categories.

