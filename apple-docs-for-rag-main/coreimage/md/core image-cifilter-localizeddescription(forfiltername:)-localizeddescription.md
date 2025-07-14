

- Core Image
- CIFilter
-  localizedDescription(forFilterName:) 

Type Method

# localizedDescription(forFilterName:)

Returns the localized description of a filter for display in the user interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func localizedDescription(forFilterName filterName: String) -> String?
```

## Parameters 

`filterName`  

The filter name.

## Return Value

The localized description of the filter.

## See Also

### Getting Localized Information for Registered Filters

class func localizedName(forFilterName: String) -> String?

Returns the localized name for the specified filter name.

class func localizedName(forCategory: String) -> String

Returns the localized name for the specified filter category.

class func localizedReferenceDocumentation(forFilterName: String) -> URL?

Returns the location of the localized reference documentation that describes the filter.

