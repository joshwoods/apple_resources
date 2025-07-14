

- Core Image
- CIFilter
-  filterNames(inCategories:) 

Type Method

# filterNames(inCategories:)

Returns an array of all published filter names that match all the specified categories.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class func filterNames(inCategories categories: [String]?) -> [String]
```

## Parameters 

`categories`  

One or more of the filter category keys defined in Filter Category Keys. Pass `nil` to get all filters in all categories.

## Return Value

An array that contains all published filter names that match all the categories specified by the `categories` argument.

## Discussion

When you pass more than one filter category, this method returns the intersection of the filters in the categories. For example, if you pass the categories kCICategoryBuiltIn and kCICategoryColorAdjustment, you obtain all the filters that are members of both the built-in and color adjustment categories. But if you pass in `kCICategoryGenerator` and kCICategoryStylize, you will not get any filters returned to you because there are no filters that are members of both the generator and stylize categories. If you want to obtain all stylize and generator filters, you must call the `filterNamesInCategories:` method for each category separately and then merge the results.

## See Also

### Accessing Registered Filters

class func filterNames(inCategory: String?) -> [String]

Returns an array of all published filter names in the specified category.

