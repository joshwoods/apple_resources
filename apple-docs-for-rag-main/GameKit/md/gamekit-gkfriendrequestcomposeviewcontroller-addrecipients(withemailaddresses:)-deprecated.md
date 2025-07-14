

- GameKit
- GKFriendRequestComposeViewController
-  addRecipients(withEmailAddresses:) Deprecated

Instance Method

# addRecipients(withEmailAddresses:)

Adds recipients based on their email addresses.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func addRecipients(withEmailAddresses emailAddresses: [String])
```

Deprecated

No longer supported.

## Parameters 

`emailAddresses`  

An array with one or more NSString objects, each containing an email address.

## Discussion

If you do not add at least once recipient, the recipients field is selected when the view controller is presented so that the player can type a list of recipients. Adding more players than defined by the maxNumberOfRecipients() property causes an exception to be thrown.

## See Also

### Adding Recipients

func addRecipientPlayers([GKPlayer])

Adds recipients based on their Game Center player identifiers.

Deprecated

func addRecipients(withPlayerIDs: [String])

Adds recipients based on their Game Center player identifiers.

Deprecated

