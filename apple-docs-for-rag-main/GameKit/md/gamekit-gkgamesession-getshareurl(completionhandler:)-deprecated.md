

- GameKit
- GKGameSession
-  getShareURL(completionHandler:) Deprecated

Instance Method

# getShareURL(completionHandler:)

Retrieves the URL used to share a game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func getShareURL(completionHandler: @escaping (URL?, (any Error)?) -> Void)
```

``` source
func shareURL() async throws -> URL
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`completionHandler`  

A block that is called after the shared URL has been retrieved.

url  
An `NSURL` object that contains the URL sent to other players in order to invite them to a game session.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## Discussion

When a player clicks the Share or Invite button in your app, they have indicated they want to interact with another player. This method to retrieves a `URL` used to invite other players into the current game session.

The completion handler for this method returns an optional `URL` and `Error`. After ensuring you have a valid `URL`, you should immediately present the player with the option to share their game session by sending the `URL` to another player or friend. This is accomplished by configuring a UIActivityViewController and presenting it. You must implicitly unwrap the `URL` when creating the activity view controller. For example, the listing below presents the shared URL on an iPad.

```
@IBAction func invitePlayerWithMessages(sender: UIButton) {
        myGameSession.getShareURL(completionHandler:  { (url, error) in
            if error == nil {
                let activityVC = UIActivityViewController.init(activityItems: [url!], applicationActivities: nil)
                activityVC.popoverPresentationController?.sourceView = sender
                self.present(activityVC, animated: true, completion: nil)

            } else {
                // .. Process the error
            }
        })
    }
```

After the URL has been shared, your app must handle any requests to join the game session.

