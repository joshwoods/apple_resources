

- TVUIKit
- TVDigitEntryViewController
-  clearEntry(animated:) 

Instance Method

# clearEntry(animated:)

Removes all digits from the digit entry view.

tvOS 12.0+

``` source
@MainActor
func clearEntry(animated: Bool)
```

## Parameters 

`animated`  

A Boolean value indicating whether the digit entry view animates when the digits are cleared.

## Discussion

The digit entry view animates the digit removal when the `animated` parameter is `YES`.

## See Also

### Entering Information

var entryCompletionHandler: (String) -> Void

A completion handler that cues the app that the user has entered the required number of digits for the digit entry view.

