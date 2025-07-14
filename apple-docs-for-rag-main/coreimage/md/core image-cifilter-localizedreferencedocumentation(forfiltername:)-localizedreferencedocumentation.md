

- Core Image
- CIFilter
-  localizedReferenceDocumentation(forFilterName:) 

Type Method

# localizedReferenceDocumentation(forFilterName:)

Returns the location of the localized reference documentation that describes the filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func localizedReferenceDocumentation(forFilterName filterName: String) -> URL?
```

## Parameters 

`filterName`  

The filter name.

## Return Value

A URL that specifies the location of the localized documentation, or `nil` if the filter does not provide localized reference documentation.

## Discussion

The URL can be a local file or a remote document on a web server. Because filters created prior to OS X v10.5 could return `nil`, you should be make sure that your code handles this case gracefully.

## See Also

### Getting Localized Information for Registered Filters

class func localizedName(forFilterName: String) -> String?

Returns the localized name for the specified filter name.

class func localizedName(forCategory: String) -> String

Returns the localized name for the specified filter category.

class func localizedDescription(forFilterName: String) -> String?

Returns the localized description of a filter for display in the user interface.

