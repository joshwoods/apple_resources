

- GameKit
-  GKPeerPickerController Deprecated

Class

# GKPeerPickerController

Provides a standard user interface to allow one iOS device to discover and connect to another.

visionOS 1.0–1.0Deprecated

``` source
class GKPeerPickerController
```

Deprecated

Use the MCBrowserViewController class in the Multipeer Connectivity framework instead.

## Overview

The result is a configured GKSession object connecting the two devices. To use a GKPeerPickerController object, your application creates the controller, adds a delegate, configures the allowed connection types, and then shows the peer picker. The delegate is called as the user makes selections within the peer picker interface.

In iOS 3.0, the peer picker can be configured to select between Bluetooth and Internet connections.

Important

Although users can select Internet connections in the peer picker, GKPeerPickerController has no user interface for configuring them. If your application configures the peer picker to allow Internet connections, your application must also dismiss the peer picker and present its own interface to configure an Internet connection.

On iOS 3.0, your application should release the peer picker object after it dismisses the peer picker dialog. On iOS 3.1 or later, your application may release the peer picker after it is shown to the user. If you do this, the peer picker controller is automatically deallocated after the dialog is dismissed.

## Topics

### Setting and Getting the Delegate

var delegate: (any GKPeerPickerControllerDelegate)?

The delegate of the peer picker controller.

### Displaying the Picker Dialog

func dismiss()

Hides the peer picker dialog.

func show()

Displays the peer picker dialog to the user.

var isVisible: Bool

A Boolean value that indicates whether the picker dialog is visible.

### Configuring Connectivity Options

var connectionTypesMask: GKPeerPickerConnectionType

A mask that determines the types of connections a dialog presents to the user.

### Constants

enum GKPeerPickerConnectionType

Network connections available to the peer picker dialog.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

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

class GKFriendRequestComposeViewController

Your game uses the `GKFriendRequestComposeViewController` class to present a screen that allows the local player to send friend requests to other players.

Deprecated

class GKLeaderboardViewController

The `GKLeaderboardViewController` class provides a standard user interface that displays leaderboard scores to the player. If the GKGameCenterViewController class is available, you should use it instead.

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

