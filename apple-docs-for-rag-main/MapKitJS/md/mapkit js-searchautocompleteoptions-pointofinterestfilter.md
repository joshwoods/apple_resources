

- MapKit JS
- SearchAutocompleteOptions
-  pointOfInterestFilter 

Instance Property

# pointOfInterestFilter

A filter used to include or exclude point of interest categories in search results.

MapKit JS 5.32.2+

``` source
attribute mapkit.PointOfInterestFilter pointOfInterestFilter;
```

## Discussion

If you provide a mapkit.PointOfInterestFilter and set includePointsOfInterest to `false` in the constructor, the filter overrides the Boolean value, and the search returns points of interest allowed by the filter.

To include or exclude all points of interest use `filterIncludingAllCategories` or `filterExcludingAllCategories`, respectively.

