

- AVFoundation
- AVTextStyleRule
-  textStyleRules(fromPropertyList:) 

Type Method

# textStyleRules(fromPropertyList:)

Creates an array of text style rule objects from the specified property-list object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func textStyleRules(fromPropertyList plist: Any) -> [AVTextStyleRule]?
```

## Parameters 

`plist`  

A property-list object containing the text style data.

## Return Value

An array of `AVTextStyleRule` objects corresponding to the style information in the property-list object.

## Discussion

Use this method to create new text style rule objects based on data you previously converted to a property-list format using the propertyList(for:) class method.

## See Also

### Creating and Initializing Style Rules

convenience init?(textMarkupAttributes: [String : Any])

Creates a text style rule object with the specified style attributes.

init?(textMarkupAttributes: [String : Any], textSelector: String?)

Creates a text style rule object with the specified style attributes and text range information.

