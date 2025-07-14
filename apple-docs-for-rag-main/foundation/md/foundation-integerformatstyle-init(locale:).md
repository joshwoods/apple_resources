

- Foundation
- IntegerFormatStyle
-  init(locale:) 

Initializer

# init(locale:)

Creates an integer format style that uses the given locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(locale: Locale = .autoupdatingCurrent)
```

## Parameters 

`locale`  

The locale to use when formatting or parsing integers. Defaults to autoupdatingCurrent.

## Discussion

Create an IntegerFormatStyle when you intend to apply a given style to multiple integers. The following example creates a style that uses the `en_US` locale, which uses three-based grouping and comma separators. It then applies this style to all the integers in an array.

```
let enUSstyle = IntegerFormatStyle(locale: Locale(identifier: "en_US"))
let nums = [100, 1000, 10000, 100000, 1000000]
let formattedNums = nums.map { enUSstyle.format($0) } // ["100", "1,000", "10,000", "100,000", "1,000,000"]
```

To format a single integer, you can use the BinaryInteger instance method formatted(_:), passing in an instance of IntegerFormatStyle.

