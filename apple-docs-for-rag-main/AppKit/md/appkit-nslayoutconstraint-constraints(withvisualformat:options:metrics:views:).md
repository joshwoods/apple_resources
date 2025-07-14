

- AppKit
- NSLayoutConstraint
-  constraints(withVisualFormat:options:metrics:views:) 

Type Method

# constraints(withVisualFormat:options:metrics:views:)

Creates constraints described by an ASCII art-like visual format string.

macOS 10.7+

``` source
class func constraints(
    withVisualFormat format: String,
    options opts: NSLayoutConstraint.FormatOptions = [],
    metrics: [String : Any]?,
    views: [String : Any]
) -> [NSLayoutConstraint]
```

## Parameters 

`format`  

The format specification for the constraints. For more information, see Auto Layout Cookbook in Auto Layout Guide.

`opts`  

Options describing the attribute and the direction of layout for all objects in the visual format string.

`metrics`  

A dictionary of constants that appear in the visual format string. The dictionary’s keys must be the string values used in the visual format string. Their values must be NSNumber objects.

`views`  

A dictionary of views that appear in the visual format string. The keys must be the string values used in the visual format string, and the values must be the view objects.

## Return Value

An array of constraints that, combined, express the constraints between the provided views and their parent view as described by the visual format string. The constraints are returned in the same order they were specified in the visual format string.

## Discussion

The language used for the visual format string is described in Auto Layout Cookbook in Auto Layout Guide.

## See Also

### Related Documentation

Auto Layout Guide

### Creating constraints

convenience init(item: Any, attribute: NSLayoutConstraint.Attribute, relatedBy: NSLayoutConstraint.Relation, toItem: Any?, attribute: NSLayoutConstraint.Attribute, multiplier: CGFloat, constant: CGFloat)

Creates a constraint that defines the relationship between the specified attributes of the given views.

