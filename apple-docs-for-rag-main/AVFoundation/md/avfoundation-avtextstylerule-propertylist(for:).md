

- AVFoundation
- AVTextStyleRule
-  propertyList(for:) 

Type Method

# propertyList(for:)

Converts one or more text style rules into a serializable property list object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func propertyList(for textStyleRules: [AVTextStyleRule]) -> Any
```

## Parameters 

`textStyleRules`  

An array of `AVTextStyleRule` objects to write to the property list.

## Return Value

A property-list object that you can pass to the PropertyListSerialization serialization routines.

## Discussion

The property-list object returned by this method can be written to disk and stored persistently.

