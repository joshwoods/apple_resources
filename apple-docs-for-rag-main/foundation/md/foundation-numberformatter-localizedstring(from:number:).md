

- Foundation
- NumberFormatter
-  localizedString(from:number:) 

Type Method

# localizedString(from:number:)

Returns a localized number string with the specified style.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localizedString(
    from num: NSNumber,
    number nstyle: NumberFormatter.Style
) -> String
```

## Parameters 

`num`  

The number to localize

`nstyle`  

The localization style to use. See NumberFormatter.Style for the supported values.

## Return Value

An appropriately formatted `NSString`.

## See Also

### Converting Between Numbers and Strings

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, range: UnsafeMutablePointer&lt;NSRange>?) throws

Returns by reference a cell-content object after creating it from a range of characters in a given string.

func number(from: String) -> NSNumber?

Returns an NSNumber object created by parsing a given string.

func string(from: NSNumber) -> String?

Returns a string containing the formatted value of the provided number object.

