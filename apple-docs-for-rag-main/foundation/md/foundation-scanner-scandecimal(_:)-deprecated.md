

- Foundation
- Scanner
-  scanDecimal(\_:) Deprecated

Instance Method

# scanDecimal(\_:)

Scans for an `NSDecimal` value, returning a found value by reference.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–13.0Deprecated

``` source
func scanDecimal(_ dcm: UnsafeMutablePointer?) -> Bool
```

## Parameters 

`dcm`  

Upon return, contains the scanned value. See the NSDecimalNumber class specification for more information about `NSDecimal` values.

## Return Value

true if the receiver finds a valid `NSDecimal` representation, otherwise false.

## Discussion

Invoke this method with `NULL` as `decimalValue` to simply scan past an `NSDecimal` representation.

## See Also

### Scanning Numeric Values

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

func scanInt32(UnsafeMutablePointer&lt;Int32>?) -> Bool

Scans for an int value from a decimal representation, returning a found value by reference.

Deprecated

func scanInt64(UnsafeMutablePointer&lt;Int64>?) -> Bool

Scans for a long long value from a decimal representation, returning a found value by reference.

func scanUnsignedLongLong(UnsafeMutablePointer&lt;UInt64>?) -> Bool

Scans for an unsigned long long value from a decimal representation, returning a found value by reference.

