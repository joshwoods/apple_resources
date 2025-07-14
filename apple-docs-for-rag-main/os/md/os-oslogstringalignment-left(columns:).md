

- os
- OSLogStringAlignment
-  left(columns:) 

Type Method

# left(columns:)

Aligns the value on the left side of a column with the specified width.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func left(columns: @autoclosure @escaping () -> Int) -> OSLogStringAlignment
```

## Parameters 

`columns`  

The width of the item in characters.

## Return Value

A string-alignment structure with the specified value.

## See Also

### Getting a Custom String Alignment

static func right(columns: @autoclosure () -> Int) -> OSLogStringAlignment

Aligns the value on the right side of a column with the specified width.

