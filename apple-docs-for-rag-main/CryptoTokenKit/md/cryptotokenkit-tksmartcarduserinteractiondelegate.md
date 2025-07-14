

- CryptoTokenKit
-  TKSmartCardUserInteractionDelegate 

Protocol

# TKSmartCardUserInteractionDelegate

The interface implemented by a Smart Card user interaction delegate to handle user interaction events.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
protocol TKSmartCardUserInteractionDelegate
```

## Topics

### Delegate Methods

func characterEntered(in: TKSmartCardUserInteraction)

Tells the delegate that a valid character has been entered.

func correctionKeyPressed(in: TKSmartCardUserInteraction)

Tells the delegate that a correction key has been pressed.

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

## See Also

### Handling User Interaction Events

var delegate: (any TKSmartCardUserInteractionDelegate)?

The delegate for observing events that occur during the user interaction.

