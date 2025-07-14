

- Foundation
- Scanner
-  scanInt32(\_:) Deprecated

Instance Method

# scanInt32(\_:)

Scans for an int value from a decimal representation, returning a found value by reference.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
func scanInt32(_ result: UnsafeMutablePointer?) -> Bool
```

## Parameters 

`result`  

Upon return, contains the scanned value. Contains `INT_MAX` or `INT_MIN` on overflow.

## Return Value

true if the receiver finds a valid decimal integer representation, otherwise false. Overflow is considered a valid integer representation.

## Discussion

Skips past excess digits in the case of overflow, so the receiver’s position is past the entire decimal representation.

Invoke this method with `NULL` as `intValue` to simply scan past a decimal integer representation.

## See Also

### Related Documentation

var intValue: Int32

The integer value of the string.

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

func scanHexFloat(UnsafeMutablePointer&lt;Float>?) -> Bool

Scans for a double value from a hexadecimal representation, returning a found value by reference.

func scanHexInt32(UnsafeMutablePointer&lt;UInt32>?) -> Bool

Scans for an unsigned value from a hexadecimal representation, returning a found value by reference.

Deprecated

func scanHexInt64(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for a long long value from a hexadecimal representation, returning a found value by reference.

func scanInt(UnsafeMutablePointer&lt;Int>?) -> Bool

Scans for an NSInteger value from a decimal representation, returning a found value by reference

func scanInt64(UnsafeMutablePointer&lt;Int64>?) -> Bool

Scans for a long long value from a decimal representation, returning a found value by reference.

func scanUnsignedLongLong(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for an unsigned long long value from a decimal representation, returning a found value by reference.

