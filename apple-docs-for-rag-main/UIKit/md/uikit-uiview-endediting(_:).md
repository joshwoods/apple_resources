

- UIKit
- UIView
-  endEditing(\_:) 

Instance Method

# endEditing(\_:)

Causes the view (or one of its embedded text fields) to resign the first responder status.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func endEditing(_ force: Bool) -> Bool
```

## Parameters 

`force`  

Specify true to force the first responder to resign, regardless of whether it wants to do so.

## Return Value

true if the view resigned the first responder status or false if it did not.

## Discussion

This method looks at the current view and its subview hierarchy for the text field that is currently the first responder. If it finds one, it asks that text field to resign as first responder. If the `force` parameter is set to true, the text field is never even asked; it is forced to resign.

