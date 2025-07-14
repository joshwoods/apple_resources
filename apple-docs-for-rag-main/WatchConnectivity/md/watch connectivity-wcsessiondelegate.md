

- Watch Connectivity
-  WCSessionDelegate 

Protocol

# WCSessionDelegate

A delegate protocol that defines methods for receiving messages sent by a WCSession object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 2.0+

``` source
protocol WCSessionDelegate : NSObjectProtocol
```

## Overview

Session objects are used to communicate between a WatchKit extension and the companion iOS app on a paired and active iPhone. When configuring your session object, you must specify a delegate object that implements this protocol. The session calls your delegate methods to deliver incoming data from the counterpart app and to manage session-related changes.

Most methods of this protocol are optional. You implement the methods you need to respond to the data transfer operations that your apps support. However, apps must implement the session(_:activationDidCompleteWith:error:) method, supporting asynchronous activation. On iOS, you must also implement the sessionDidBecomeInactive(_:) and sessionDidDeactivate(_:) methods, supporting multiple Apple Watches.

The WCSession object calls the methods of its delegate serially, so your method implementations do not need to be reentrant. Immediate messages can be sent only while both the WatchKit extension and iOS app are running. By contrast, context updates and file transfers can be initiated at any time and delivered in the background to the other device. All transfers are delivered in the order in which they were sent.

Note

The methods of this protocol are called on a background thread of your app, so any code you write should be written with that fact in mind. In particular, if your method implementations initiate modifications to your app’s interface, make sure to redirect those modifications to your app’s main thread.

### Supporting Communication with Multiple Apple Watches

An iPhone running iOS 9.3 or later may pair with more than one Apple Watch running watchOS 2.2 or later. Implement the following methods in your session delegate:

- session(_:activationDidCompleteWith:error:)

- sessionDidBecomeInactive(_:) (iOS only)

- sessionDidDeactivate(_:) (iOS only)

Use the activation-related methods to track the activation state of the session in your iOS app. With Auto Switch enabled on the user’s iPhone, the session automatically moves to the inactive state when the user puts on a different Apple Watch than the one that is currently active. (If Auto Switch is disabled, the user must manually select which watch is active.) While your iOS app is in the inactive state, the system finishes delivering any data that has been received before moving your app to the deactivated state. While inactive or deactivated, you cannot initiate any new transfers. When your iOS app reaches the deactivated state, call the session’s activate() method again to connect to the new Apple Watch.

For more information about the flow of messages when a user switches from one Apple Watch to another, see WCSession.

## Topics

### Managing Session Activation

func session(WCSession, activationDidCompleteWith: WCSessionActivationState, error: (any Error)?)

Tells the delegate that the session has finished activating.

**Required**

func sessionDidBecomeInactive(WCSession)

Tells the delegate that the session will stop communicating with the current Apple Watch.

**Required**

func sessionDidDeactivate(WCSession)

Tells the delegate that the session has delivered all the data from the previous session, and that communication with the Apple Watch has ended.

**Required**

### Managing State Changes

func sessionWatchStateDidChange(WCSession)

Indicates a change to the counterpart’s information.

func sessionReachabilityDidChange(WCSession)

Indicates a change to the counterpart’s reachability status.

func sessionCompanionAppInstalledDidChange(WCSession)

Indicates a change to the companion app’s installed state.

### Receiving Context Data

func session(WCSession, didReceiveApplicationContext: [String : Any])

Tells the delegate that the session has received context data from the counterpart.

### Receiving Immediate Messages

func session(WCSession, didReceiveMessage: [String : Any])

Tells the delegate that an immediate message has arrived.

func session(WCSession, didReceiveMessage: [String : Any], replyHandler: ([String : Any]) -> Void)

Tells the delegate that an immediate message has arrived, and it requires a response.

func session(WCSession, didReceiveMessageData: Data)

Tells the delegate that an immediate data message has arrived.

func session(WCSession, didReceiveMessageData: Data, replyHandler: (Data) -> Void)

Tells the delegate that an immediate data message has arrived, and it requires a response.

### Managing Data Dictionary Transfers

func session(WCSession, didReceiveUserInfo: [String : Any])

Tells the delegate that the session successfully received a data directory from its counterpart.

func session(WCSession, didFinish: WCSessionUserInfoTransfer, error: (any Error)?)

Tells the delegate that a data transfer operation has finished successfully or ended because of an error.

### Managing File Transfers

func session(WCSession, didReceive: WCSessionFile)

Tells the delegate that the session successfully received a file from its counterpart.

func session(WCSession, didFinish: WCSessionFileTransfer, error: (any Error)?)

Tells the delegate that a file transfer has finished successfully or ended because of an error.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

class WCSession

The object that initiates communication between a WatchKit extension and its companion iOS app.

