

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.fieldStateChanged(info:) 

Case

# CredentialSession.Event.fieldStateChanged(info:)

The state of the NFC RF field changed during card emulation.

iOS 18.1+iPadOS 18.1+

``` source
case fieldStateChanged(info: CredentialSession.NFCFieldInformation)
```

## Discussion

The credential session sends an initial event with the current field state when entering the card emulation state. The session then sends further events if the field state changes. The session only publishes this event when it’s in the card emulation state.

You can only receive this event if you have acquired the CredentialSession.PresentmentIntentAssertion.

## See Also

### NFC field events

enum NFCFieldInformation

The state of an NFC RF field.

