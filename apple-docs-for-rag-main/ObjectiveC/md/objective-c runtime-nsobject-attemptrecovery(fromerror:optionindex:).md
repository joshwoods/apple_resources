

- Objective-C Runtime
- NSObject
-  attemptRecovery(fromError:optionIndex:) 

Instance Method

# attemptRecovery(fromError:optionIndex:)

Implemented to attempt a recovery from an error noted in an application-modal dialog.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func attemptRecovery(
    fromError error: any Error,
    optionIndex recoveryOptionIndex: Int
) -> Bool
```

## Parameters 

`error`  

An NSError object that describes the error, including error recovery options.

`recoveryOptionIndex`  

The index of the user selected recovery option in `error`’s localized recovery array.

## Return Value

YES if the error recovery was completed successfully, NO otherwise.

## Discussion

Invoked when an error alert is been presented to the user in an application-modal dialog, and the user has selected an error recovery option specified by `error`.

