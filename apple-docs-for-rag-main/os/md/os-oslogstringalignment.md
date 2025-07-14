

- os
-  OSLogStringAlignment 

Structure

# OSLogStringAlignment

The alignment options for interpolated strings.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogStringAlignment
```

## Mentioned in 

Generating Log Messages from Your Code

## Topics

### Getting the Standard Alignment

static var none: OSLogStringAlignment

No alignment.

### Getting a Custom String Alignment

static func left(columns: @autoclosure () -> Int) -> OSLogStringAlignment

Aligns the value on the left side of a column with the specified width.

static func right(columns: @autoclosure () -> Int) -> OSLogStringAlignment

Aligns the value on the right side of a column with the specified width.

