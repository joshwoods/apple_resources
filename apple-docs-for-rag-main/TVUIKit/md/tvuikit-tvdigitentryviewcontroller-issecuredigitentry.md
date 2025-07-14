

- TVUIKit
- TVDigitEntryViewController
-  isSecureDigitEntry 

Instance Property

# isSecureDigitEntry

A Boolean value that indicates whether an entered digit is immediately obscured.

tvOS 12.0+

``` source
@MainActor
var isSecureDigitEntry: Bool { get set }
```

## Discussion

The defualt value is `NO`.

## See Also

### Configuring the Digit Entry View

var numberOfDigits: Int

The number of required digits.

var titleText: String?

The title of the digit entry view.

var promptText: String?

A prompt that displays any additional required information.

