

- CKTool JS
- CKDBQueryFilter
-  radiusInKilometers 

Instance Property

# radiusInKilometers

A radius used to determine whether a field that is a location is inside a circular area.

CKTool JS 1.2.15+

``` source
attribute Double? radiusInKilometers;
```

## Discussion

This property is only used if the record field indicated by `fieldName` has a value that is a `CKDBLocation` type. When used, the center of the circle is `fieldValue` and the radius is distance.

