

- Foundation
- Scanner
-  scanHexFloat(\_:) 

Instance Method

# scanHexFloat(\_:)

Scans for a double value from a hexadecimal representation, returning a found value by reference.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func scanHexFloat(_ result: UnsafeMutablePointer?) -> Bool
```

## Parameters 

`result`  

Upon return, contains the scanned value. Contains `HUGE_VAL` or `–HUGE_VAL` on overflow, or `0.0` on underflow.

## Return Value

true if the receiver finds a valid float-point representation, otherwise false. Overflow or underflow are both considered valid floating-point representations.

## Discussion

This corresponds to `%a` or `%A` formatting. The hexadecimal float representation must be preceded by `0x` or `0X`.

Skips past excess digits in the case of overflow, so the scanner’s position is past the entire floating-point representation.

Invoke this method with `NULL` as `result` to simply scan past a hexadecimal float representation.

## See Also

### Scanning Numeric Values

func scanDecimal(UnsafeMutablePointer&lt;Decimal>?) -> Bool

Scans for an `NSDecimal` value, returning a found value by reference.

Deprecated

func scanDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value, returning a found value by reference.

Deprecated

func scanFloat(UnsafeMutablePointer&lt;Float>?) -> Bool

Scans for a float value, returning a found value by reference.

Deprecated

func scanHexDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value from a hexadecimal representation, returning a found value by reference.

func scanHexInt32(UnsafeMutablePointer&lt;UInt32>?) -> Bool

Scans for an unsigned value from a hexadecimal representation, returning a found value by reference.

Deprecated

func scanHexInt64(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for a long long value from a hexadecimal representation, returning a found value by reference.

func scanInt(UnsafeMutablePointer&lt;Int>?) -> Bool

Scans for an NSInteger value from a decimal representation, returning a found value by reference

func scanInt32(UnsafeMutablePointer&lt;Int32>?) -> Bool

Scans for an int value from a decimal representation, returning a found value by reference.

Deprecated

func scanInt64(UnsafeMutablePointer&lt;Int64>?) -> Bool

Scans for a long long value from a decimal representation, returning a found value by reference.

func scanUnsignedLongLong(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for an unsigned long long value from a decimal representation, returning a found value by reference.

