

- Core NFC
-  NFCWindowSceneDelegate 

Protocol

# NFCWindowSceneDelegate

A protocol to notify your app’s user interface about NFC-related events.

CoreNFCUIKitiOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
protocol NFCWindowSceneDelegate
```

## Overview

When the device is eligible to receive NFC-related events, use this protocol to update your user interface. The received NFCWindowSceneEvent indicates whether the event represents the presence of a card reader or a gesture to initiate a contactless transaction by the person using the app.

You typically add conformance to this protocol in your app’s main scene delegate, where you already conform to UIWindowSceneDelegate.

## Topics

### Handling events

func windowScene(UIWindowScene, didReceiveNFCWindowSceneEvent: NFCWindowSceneEvent)

Informs your app that the system has received an NFC-related event.

**Required**

enum NFCWindowSceneEvent

An NFC-related event that your app uses to update its user interface.

## See Also

### NFC window scenes

enum NFCWindowSceneEvent

An NFC-related event that your app uses to update its user interface.

