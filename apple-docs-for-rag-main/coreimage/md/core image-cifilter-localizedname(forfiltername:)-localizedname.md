

- Core Image
- CIFilter
-  localizedName(forFilterName:) 

Type Method

# localizedName(forFilterName:)

Returns the localized name for the specified filter name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func localizedName(forFilterName filterName: String) -> String?
```

## Parameters 

`filterName`  

A filter name.

## Return Value

The localized name for the filter.

## See Also

### Getting Localized Information for Registered Filters

class func localizedName(forCategory: String) -> String

Returns the localized name for the specified filter category.

class func localizedDescription(forFilterName: String) -> String?

Returns the localized description of a filter for display in the user interface.

class func localizedReferenceDocumentation(forFilterName: String) -> URL?

Returns the location of the localized reference documentation that describes the filter.

