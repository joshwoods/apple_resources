

- GameKit
-  GKFriendRequestComposeViewController Deprecated

Class

# GKFriendRequestComposeViewController

Your game uses the `GKFriendRequestComposeViewController` class to present a screen that allows the local player to send friend requests to other players.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class GKFriendRequestComposeViewController
```

Deprecated

No longer supported.

## Overview

Important

Your game must authenticate a local player before you can use any Game Center classes. If there is no authenticated player, your game receives a GKError.Code.notAuthenticated error. For more information, see Authenticating a player.

To show a friend request, initialize a new `GKFriendRequestComposeViewController` object and set the delegate. Optionally, you can customize the request by adding a text message or a list of recipients. Then, present the new view controller and wait for the delegate to be called. Once the delegate is called, dismiss the view controller.

On iOS, you present and dismiss the view controller from another view controller in your game, using the methods provided by the UIViewController class. In macOS, you use the GKDialogController class to present and dismiss the view controller. The listing below shows one way your view controller can allow a player to send a request to other players. For this method, an array of GKPlayer objects is passed in as a parameter. The method instantiates a `GKFriendRequestComposeViewController` object, sets its delegate, and adds the list of players intended to receive the invitation. The view controller then presents the friend request and returns.

```
```

### Subclassing Notes

The GKFriendRequestComposeViewController class is not intended to be subclassed.

## Topics

### Determining the Maximum Number of Recipients

class func maxNumberOfRecipients() -> Int

Returns the maximum number of recipients permitted in a single request.

### Delegate

var composeViewDelegate: (any GKFriendRequestComposeViewControllerDelegate)?

The view controller’s delegate

### Adding Recipients

func addRecipients(withEmailAddresses: [String])

Adds recipients based on their email addresses.

func addRecipientPlayers([GKPlayer])

Adds recipients based on their Game Center player identifiers.

func addRecipients(withPlayerIDs: [String])

Adds recipients based on their Game Center player identifiers.

### Setting an Invitation Message

func setMessage(String?)

Sets the text message included in the friend invitation.

## Relationships

### Inherits From

- NSViewController
- UINavigationController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKViewController
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated classes

class GKAchievementViewController

An `GKAchievementViewController` object provides a standard user interface to display achievement progress for the local player. If the GKGameCenterViewController class is available, you should use it instead.

Deprecated

class GKChallengeEventHandler

The `GKChallengeEventHandler` class is used to respond to events related to challenges sent or received by the local player.

Deprecated

class GKChallengesViewControllerDeprecated

class GKCloudPlayer

The object representing the currently signed-in iCloud user.

Deprecated

class GKGameSession

A game session you can use to save game data, invite other players, and create turn-based and real-time game apps.

Deprecated

class GKGameSessionSharingViewController

A user interface you can use to invite other users into a tvOS game session.

Deprecated

class GKLeaderboardViewController

The `GKLeaderboardViewController` class provides a standard user interface that displays leaderboard scores to the player. If the GKGameCenterViewController class is available, you should use it instead.

Deprecated

class GKPeerPickerController

Provides a standard user interface to allow one iOS device to discover and connect to another.

Deprecated

class GKScore

An object containing information for a score that was earned by the player.

Deprecated

class GKSession

A GKSession object provides the ability to discover and connect to nearby iOS devices using Bluetooth or Wi-fi.

Deprecated

class GKTurnBasedEventHandler

The GKTurnBasedEventHandler class is used to respond to important messages related to turn-based matches. To use it, call the shared() class method to get the singleton instance and assign an object that implements the GKTurnBasedEventHandlerDelegate protocol to its delegate property. All methods are called on the main thread.

Deprecated

class GKVoiceChat

A voice channel that allows players to speak with each other in a multiplayer game.

Deprecated

class GKVoiceChatService

The GKVoiceChatService class allows your application to connect two iOS devices into a voice chat.

Deprecated

