

- GameKit
- GKFriendRequestComposeViewController
-  addRecipients(withPlayerIDs:) Deprecated

Instance Method

# addRecipients(withPlayerIDs:)

Adds recipients based on their Game Center player identifiers.

iOS 4.2–8.0DeprecatediPadOS 4.2–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func addRecipients(withPlayerIDs playerIDs: [String])
```

## Parameters 

`playerIDs`  

An array with one or more NSString objects, each containing an player identifier.

## Discussion

If you do not add at least once recipient, the recipients field is selected when the view controller is presented so that the player can type a list of recipients.

## See Also

### Adding Recipients

func addRecipients(withEmailAddresses: [String])

Adds recipients based on their email addresses.

Deprecated

func addRecipientPlayers([GKPlayer])

Adds recipients based on their Game Center player identifiers.

Deprecated

