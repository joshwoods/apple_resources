

- UIKit
- NSTextTab
-  columnTerminators(for:) 

Type Method

# columnTerminators(for:)

Returns the column terminators for the specified locale.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func columnTerminators(for aLocale: Locale?) -> CharacterSet
```

## Parameters 

`aLocale`  

The locale to use when determining the terminators. Specify `nil` to use the system’s current locale. You can get the user’s locale using the current method of NSLocale.

## Return Value

The characters for the column terminators.

## Discussion

The returned value can be used as the value for columnTerminators to make a decimal tab stop.

## See Also

### Getting text tab information

var alignment: NSTextAlignment

The text alignment of the text tab.

var options: [NSTextTab.OptionKey : Any]

The dictionary of attributes for the text tab.

