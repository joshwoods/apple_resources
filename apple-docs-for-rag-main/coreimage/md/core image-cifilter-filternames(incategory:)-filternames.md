

- Core Image
- CIFilter
-  filterNames(inCategory:) 

Type Method

# filterNames(inCategory:)

Returns an array of all published filter names in the specified category.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func filterNames(inCategory category: String?) -> [String]
```

## Parameters 

`category`  

A string object that specifies one of the filter categories defined in Filter Category Keys.

## Return Value

An array that contains all published names of the filter in a category.

## See Also

### Accessing Registered Filters

class func filterNames(inCategories: [String]?) -> [String]

Returns an array of all published filter names that match all the specified categories.

