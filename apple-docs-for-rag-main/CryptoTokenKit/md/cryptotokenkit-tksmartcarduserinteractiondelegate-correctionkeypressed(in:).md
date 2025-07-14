

- CryptoTokenKit
- TKSmartCardUserInteractionDelegate
-  correctionKeyPressed(in:) 

Instance Method

# correctionKeyPressed(in:)

Tells the delegate that a correction key has been pressed.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
optional func correctionKeyPressed(in interaction: TKSmartCardUserInteraction)
```

## Parameters 

`interaction`  

The user interaction.

## See Also

### Delegate Methods

func characterEntered(in: TKSmartCardUserInteraction)

Tells the delegate that a valid character has been entered.

func validationKeyPressed(in: TKSmartCardUserInteraction)

Tells the delegate that the validation key has been pressed, indicating the end of PIN entry.

func invalidCharacterEntered(in: TKSmartCardUserInteraction)

Tells the delegate that an invalid character has been entered.

func oldPINRequested(in: TKSmartCardUserInteraction)

Tells the delegate that the old PIN needs to be entered.

func newPINRequested(in: TKSmartCardUserInteraction)

Tells the delegate that the new PIN needs to be entered.

func newPINConfirmationRequested(in: TKSmartCardUserInteraction)

Tells the delegate that the new PIN needs to be re-entered for confirmation.

