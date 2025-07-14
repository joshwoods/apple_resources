

- Foundation
- NSDataDetector
-  checkingTypes 

Instance Property

# checkingTypes

Returns the checking types for the data detector.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var checkingTypes: NSTextCheckingTypes { get }
```

## Discussion

The supported subset of checking types are specified in NSTextCheckingResult.CheckingType. Those constants can be combined using the C-bitwise OR operator.

Currently, the supported data detectors `checkingTypes` are: date, address, link, `NSTextCheckingTypePhoneNumber`, and `NSTextCheckingTypeTransitInformation`.

