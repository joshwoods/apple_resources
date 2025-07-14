

- Swift Testing
- CustomTestStringConvertible
-  testDescription 

Instance Property

# testDescription

A description of this instance to use when presenting it in a test’s output.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
var testDescription: String { get }
```

**Required** Default implementation provided.

## Discussion

Do not use this property directly. To get the test description of a value, use `Swift/String/init(describingForTest:)`.

## Default Implementations

### CustomTestStringConvertible Implementations

var testDescription: String

A description of this instance to use when presenting it in a test’s output.

