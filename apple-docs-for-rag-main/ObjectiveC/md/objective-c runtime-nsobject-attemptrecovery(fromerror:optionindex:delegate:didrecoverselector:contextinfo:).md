

- Objective-C Runtime
- NSObject
-  attemptRecovery(fromError:optionIndex:delegate:didRecoverSelector:contextInfo:) 

Instance Method

# attemptRecovery(fromError:optionIndex:delegate:didRecoverSelector:contextInfo:)

Implemented to attempt a recovery from an error noted in a document-modal sheet.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func attemptRecovery(
    fromError error: any Error,
    optionIndex recoveryOptionIndex: Int,
    delegate: Any?,
    didRecoverSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`error`  

An NSError object that describes the error, including error recovery options.

`recoveryOptionIndex`  

The index of the user selected recovery option in `error`’s localized recovery array.

`delegate`  

An object that is the modal delegate.

`didRecoverSelector`  

A selector identifying the method implemented by the modal delegate.

`contextInfo`  

Arbitrary data associated with the attempt at error recovery, to be passed to `delegate` in `didRecoverSelector`.

## Discussion

Invoked when an error alert is presented to the user in a document-modal sheet, and the user has selected an error recovery option specified by `error`. After recovery is attempted, your implementation should send `delegate` the message specified in `didRecoverSelector`, passing the provided `contextInfo`.

The `didRecoverSelector` should have the following signature:

```
```

where `didRecover` is YES if the error recovery attempt was successful; otherwise it is NO.

