

- Foundation
- NumberFormatter
-  string(from:) 

Instance Method

# string(from:)

Returns a string containing the formatted value of the provided number object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(from number: NSNumber) -> String?
```

## Parameters 

`number`  

An NSNumber object that is parsed to create the returned string object.

## Return Value

A string containing the formatted value of `number` using the receiver’s current settings.

## See Also

### Converting Between Numbers and Strings

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, range: UnsafeMutablePointer&lt;NSRange>?) throws

Returns by reference a cell-content object after creating it from a range of characters in a given string.

func number(from: String) -> NSNumber?

Returns an NSNumber object created by parsing a given string.

class func localizedString(from: NSNumber, number: NumberFormatter.Style) -> String

Returns a localized number string with the specified style.

