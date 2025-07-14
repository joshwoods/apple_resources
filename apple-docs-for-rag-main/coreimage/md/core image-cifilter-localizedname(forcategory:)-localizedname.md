

- Core Image
- CIFilter
-  localizedName(forCategory:) 

Type Method

# localizedName(forCategory:)

Returns the localized name for the specified filter category.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func localizedName(forCategory category: String) -> String
```

## Parameters 

`category`  

A filter category.

## Return Value

The localized name for the filter category.

## See Also

### Getting Localized Information for Registered Filters

class func localizedName(forFilterName: String) -> String?

Returns the localized name for the specified filter name.

class func localizedDescription(forFilterName: String) -> String?

Returns the localized description of a filter for display in the user interface.

class func localizedReferenceDocumentation(forFilterName: String) -> URL?

Returns the location of the localized reference documentation that describes the filter.

