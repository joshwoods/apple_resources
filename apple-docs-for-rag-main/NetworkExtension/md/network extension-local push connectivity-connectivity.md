

- Network Extension
-  Local push connectivity 

API Collection

# Local push connectivity

Provide functionality similar to Apple Push Notification Service when access to the wider internet is unavailable.

## Overview

Use the Local Push Connectivity API to maintain a persistent network connection to a server to alert users to Voice-over-IP (VoIP) calls and other messages. Local Push Connectivity is appropriate for use cases where an iOS device operates on a local, restricted network that doesn’t have access to APNs. The App Push Provider extension functions like a local network replacement for APNs; use it primarily to send small messages and alerts to users.

Local Push Connectivity has two components:

- NEAppPushManager is a programmatic interface for configuring the Local Push Connectivity extension. Your app creates NEAppPushManager instances to indicate on which Wi-Fi networks the extension runs. You also need to set the delegate of the NEAppPushManager so the iOS app can handle incoming calls reported by the extension.

- NEAppPushProvider is a type you subclass to create and maintain a persistent network connection to your server. When a user’s iOS device joins a Wi-Fi network that has an SSID matching a configured SSID in your NEAppPushManager instance, the system launches your app extension and instantiates the NEAppPushProvider subclass within that app extension. The framework calls your provider’s start(completionHandler:), which is your cue to establish a connection to the server. The NEAppPushManager continues to run in the background, as long as the device joins the matching SSID. When your server notifies your NEAppPushProvider of an incoming message or call, the provider alerts the user. Create this alert through either a local notification or by calling the reportIncomingCall(userInfo:) method that allows the parent iOS app to trigger CallKit.

Important

To use the Local Push Connectivity API, your app must have the Network Extensions Entitlement with the `app-push-provider` value. Request this entitlement from the Entitlement Request Page. After you receive the entitlement, apply it to both your app target and your provider extension target.

### Supporting APNs and local push connectivity in one app

An app can use both Local Push Connectivity and Apple Push Notification Service. Typically, you use Local Push Connectivity in a restricted network environment, and use APNs in an unrestricted network. Think of Local Push Connectivity as your private network replacement for APNs, and therefore limit your functionality within the push provider extension to delivering local notifications and CallKit alerts to users.

Your server determines whether to use Local Push Connectivity or APNs:

- If the server has a viable connection of the type that’s established by the client’s NEAppPushProvider, send the notification over that connection. The push provider extension acknowledges receipt of any message it receives over the connection.

- If the server doesn’t have an active connection to the NEAppPushProvider, or if the extension fails to acknowledge a message sent by the server, use APNs.

## Topics

### Essentials

class NEAppPushManager

An object that configures a push provider and manages its life cycle.

class NEAppPushProvider

An object that creates and maintains a persistent network connection to a local push server.

Maintaining a Reliable Network Connection

Implement your Local Push Connectivity app to ensure delivery of notifications.

Receiving Voice and Text Communications on a Local Network

Provide voice and text communication on a local network isolated from Apple Push Notification service by adopting Local Push Connectivity.

