

- Address Book UI
- ABNewPersonViewControllerDelegate
-  newPersonViewController(\_:didCompleteWithNewPerson:) 

Instance Method

# newPersonViewController(\_:didCompleteWithNewPerson:)

Sent when the user taps Save or Cancel. If the user tapped Save, the current address book has been saved to the Address Book database.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
func newPersonViewController(
    _ newPersonView: ABNewPersonViewController,
    didCompleteWithNewPerson person: ABRecord?
)
```

**Required**

## Parameters 

`person`  

On Save, the newly created (and saved) person record.

On Cancel, `NULL`.

## Discussion

If the user tapped Save, pending changes in the current address book (`ABAddressBook`) have been saved by the time this message is sent to the receiver.

The receiver must dismiss `newPersonViewController`.

