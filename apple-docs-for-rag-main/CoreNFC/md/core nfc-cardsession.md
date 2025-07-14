

- Core NFC
-  CardSession 

Class

# CardSession

An ISO 7816 card emulation session.

iOS 17.4+iPadOS 17.4+

``` source
class CardSession
```

## Overview

Use an instance of CardSession to perform ISO 7816-4 protocol communication with an NFC reader, receiving and responding to Application Protocol Data Units (APDUs) in your app.

CardSession supports host card emulation (HCE) transactions for in-store payments, car keys, closed-loop transit, corporate badges, hotel keys, merchant loyalty/rewards and event tickets in the European Economic Area (EEA).

Use a card session to perform card emulation when in the presence of an NFC reader. You do this by managing the session as follows:

1.  Verify that the system is eligible to use CardSession. Check `NFCReaderSession.readingAvailable` and `CardSession.isSupported` to ensure that the device supports card sessions with NFC. Also check `CardSession.isEligible` to verify that the system supports card session use in the current environment. Don’t continue unless all of these values are `true`.

2.  Create a card session with init() and begin iterating over events from the session’s eventStream. Starting the session acquires necessary system resources and posts CardSession.Event.sessionStarted to the event stream when the app acquires the NFC resource. After this, the session sends the CardSession.Event.readerDetected event when the device detects the RF field of an NFC reader.

3.  Start card emulation by calling startEmulation() when your app is ready to handle APDUs from the reader. You typically do this after receiving the CardSession.Event.readerDetected, but you can start emulation regardless of whether a reader is present. After you start emulation, the reader (if present) can communicate with the card, and emulation triggers the system modal UI to display over the app.

4.  At this point, begin receiving and processing APDUs from the event stream. Process the APDU payload in each event, generate a response, and send it with respond(response:). If you don’t respond in a timely manner to every event, the reader might treat it as a timeout condition and fail with an error.

5.  Use the alertMessage property to provide updates to the person using the app as the communication continues.

6.  If the reader disconnects, possibly because of the device moving away from the reader, handle the event CardSession.Event.readerDeselected.

7.  Stop card emulation by calling stopEmulation(status:). This shuts down the RF interface and cuts off the RF connection with a reader if one exists.

8.  Invalidate the session with invalidate(), which cleans up system resources.

The following example shows a simple interaction with a card session. It attempts to acquire both a NFCPresentmentIntentAssertion and a CardSession. If both of these succeed, it uses a `for-await-in` loop to process events from the session’s eventStream as it receives them.

```
import CoreNFC

func CardSessionSample() {
    /// A place-holder function for APDU processing. In a real app,
    /// process the received data and return a response as Data.
    let ProcessAPDU: (_: Data) -> Data = { capdu in return Data() }

    Task() {
        // Proceed only if the current device and system are able and
        // eligible to use CardSession.
        guard NFCReaderSession.readingAvailable,
              CardSession.isSupported,
              await CardSession.isEligible else {
            return
        }

        // Hold a presentment intent assertion reference to prevent the
        // default contactless app from launching. In a real app, monitor
        // presentmentIntent.isValid to ensure the assertion remains active.
        var presentmentIntent: NFCPresentmentIntentAssertion?

        let cardSession: CardSession
        do {
            presentmentIntent = try await NFCPresentmentIntentAssertion.acquire()
            cardSession = try await CardSession()
        } catch {
            /// Handle failure to acquire NFC presentment intent assertion or
            /// card session.
            return
        }

        // Iterate over events as the card session produces them.
        for try await event in cardSession.eventStream {
            switch event {
            case .sessionStarted:
                cardSession.alertMessage = String(localized: "Communicating with card reader.")
                break

            case .readerDetected:
                /// Start card emulation on first detection of an external reader.
                try await cardSession.startEmulation()

            case .readerDeselected:
                /// Stop emulation on first notification of RF link loss.
                await cardSession.stopEmulation(status: .success)

            case .received(let cardAPDU):
                do {
                    /// Call handler to process received input and produce a response.
                    let responseAPDU = ProcessAPDU(cardAPDU.payload)

                    try await cardAPDU.respond(response: responseAPDU)
                } catch {
                    /// Handle the error from respond(response:). If the error is
                    /// CardSession.Error.transmissionError, then retry by calling
                    /// CardSession.APDU.respond(response:) again.
                }

            case .sessionInvalidated(reason: _):
                cardSession.alertMessage = String(localized: "Ending communication with card reader.")
                /// Handle the reason for session invalidation.
                break
            }
        }

        presentmentIntent = nil /// Release presentment intent assertion.
    }
}
```

### Handling emulation duration

Card emulation is valid for up to 60 seconds from the startEmulation() call. Once the session timeout occurs, the eventStream posts the event CardSession.Event.sessionInvalidated(reason:) with a `reason` of CardSession.Error.maxSessionDurationReached. At this point, the session becomes invalidated.

### Using entitlements

Your app must have the following entitlements to use CardSession:

com.apple.developer.nfc.hce  
A Boolean value that indicates this app can use card sessions.

com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes  
A string array of ISO 7816 identifier strings that your app listens for when receiving the `SELECT` command from the reader. These strings can be fully-qualified Application Identifier (AID) strings, Registered Application Provider Identifier (RID) strings, or prefix strings. Any prefix strings must be at least as long as the RID.

If your app lacks a required entitlement, init() raises fatalError(_:file:line:). To avoid this, check the isSupported and isEligible properties before attempting to create a card session.

Optionally, your app may have the com.apple.developer.nfc.hce.default-contactless-app entitlement. A value of `YES` indicates that a person can use the iOS settings app to set this app as a default NFC contactless app.

For more information and to apply for these entitlements, visit HCE-based contactless transactions for banking and wallet apps in the European Economic Area.

Important

Use of this entitlement is managed by Apple. It is subject to the terms and conditions agreed to as part of the application process.

### Testing requirements

To test HCE-based contactless transactions, you’ll need to test with an iPhone and NFC hardware. CardSession requires the presence of an NFC reader, which isn’t supported in Simulator, to perform an ISO 7816 card emulation session.

To learn more about CardSession requirements, see HCE-based contactless transactions for banking and wallet apps in the European Economic Area.

## Topics

### Creating a card session

init() async throws

Creates a contactless card session.

enum Error

An error type that indicates problems with a card session.

### Determining card session availability

class var isSupported: Bool

A property that indicates whether the current device supports card session functionality.

static var isEligible: Bool

A property that indicates whether the current system supports card session functionality.

### Managing card emulation

func startEmulation() async throws

Start the card emulation and present a modal user interface to the person using the app.

enum Error

An error type that indicates problems with a card session.

func stopEmulation(status: CardSession.EmulationUIStatus) async

Stop card emulation and display a status.

enum EmulationUIStatus

The final status to show in the user interface when ending card emulation.

var isEmulationInProgress: Bool

A Boolean value that indicates whether emulation is currently active.

### Handling card events

var eventStream: CardSession.EventStream

An asynchronous sequence of events from the card session.

class EventStream

An asynchronous sequence of events produced by a card session.

enum Event

A type that enumerates events produced by a card session.

### Updating the user interface

var alertMessage: String

A message to show on the alert action sheet after card emulation starts.

### Ending a card session

func invalidate()

Invalidates the current card emulation session.

### Entitlements

com.apple.developer.nfc.hce

A Boolean value indicating whether your app can use the card session API.

com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes

An array of identifier strings the app handles with the card session API.

com.apple.developer.nfc.hce.default-contactless-app

A Boolean value indicating whether your app can be a default app for contactless NFC with the card session API.

### Classes

class APDU

An Application Programming Data Unit (APDU) received from the NFC card reader.

## See Also

### Card sessions

class NFCPresentmentIntentAssertion

An object that signals your app’s intention to make exclusive use of the device’s contactless features.

