

- TVUIKit
- TVDigitEntryViewController
-  promptText 

Instance Property

# promptText

A prompt that displays any additional required information.

tvOS 12.0+

``` source
@MainActor
var promptText: String? { get set }
```

## Discussion

The prompt text is displayed immediately below the title text.

## See Also

### Configuring the Digit Entry View

var numberOfDigits: Int

The number of required digits.

var titleText: String?

The title of the digit entry view.

var isSecureDigitEntry: Bool

A Boolean value that indicates whether an entered digit is immediately obscured.

