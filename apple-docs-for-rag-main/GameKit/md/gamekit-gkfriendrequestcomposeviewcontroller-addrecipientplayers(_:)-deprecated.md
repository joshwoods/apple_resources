

- GameKit
- GKFriendRequestComposeViewController
-  addRecipientPlayers(\_:) Deprecated

Instance Method

# addRecipientPlayers(\_:)

Adds recipients based on their Game Center player identifiers.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func addRecipientPlayers(_ players: [GKPlayer])
```

## Parameters 

`players`  

An array with one or more GKPlayer objects, each containing an player identifier.

## Discussion

If you do not add at least once recipient, the recipients field is selected when the view controller is presented so that the player can type a list of recipients. Adding more players than defined by the maxNumberOfRecipients() property causes an exception to be thrown.

## See Also

### Adding Recipients

func addRecipients(withEmailAddresses: [String])

Adds recipients based on their email addresses.

Deprecated

func addRecipients(withPlayerIDs: [String])

Adds recipients based on their Game Center player identifiers.

Deprecated

