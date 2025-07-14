

- Foundation
- Scanner
-  scanFloat(\_:) Deprecated

Instance Method

# scanFloat(\_:)

Scans for a float value, returning a found value by reference.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
func scanFloat(_ result: UnsafeMutablePointer?) -> Bool
```

## Parameters 

`result`  

Upon return, contains the scanned value. Contains `HUGE_VAL` or `–HUGE_VAL` on overflow, or `0.0` on underflow.

## Return Value

true if the receiver finds a valid floating-point representation, otherwise false. Overflow or underflow are both considered valid floating-point representations.

## Discussion

Skips past excess digits in the case of overflow, so the scanner’s position is past the entire floating-point representation.

Invoke this method with `NULL` as `floatValue` to simply scan past a float value representation. Floating-point representations are assumed to be IEEE compliant.

## See Also

### Related Documentation

var floatValue: Float

The floating-point value of the string as a `float`.

### Scanning Numeric Values

func scanDecimal(UnsafeMutablePointer&lt;Decimal>?) -> Bool

Scans for an `NSDecimal` value, returning a found value by reference.

Deprecated

func scanDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value, returning a found value by reference.

Deprecated

func scanHexDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value from a hexadecimal representation, returning a found value by reference.

func scanHexFloat(UnsafeMutablePointer&lt;Float>?) -> Bool

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

