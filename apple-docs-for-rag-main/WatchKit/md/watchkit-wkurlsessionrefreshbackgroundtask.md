

- WatchKit
-  WKURLSessionRefreshBackgroundTask 

Class

# WKURLSessionRefreshBackgroundTask

A task that responds to background URL sessions.

watchOS 3.0+

``` source
class WKURLSessionRefreshBackgroundTask
```

## Mentioned in 

Using background tasks

## Overview

Always upload and download data using a URLSession background transfer. Background transfers occur in a separate process and continue to transfer data even after your app terminates. Asynchronous uploads and downloads, on the other hand, suspend with your app. Because watchOS apps have a short runtime, you can’t guarantee that an asynchronous transfer finishes before the app suspends. For more information on background transfers, see Downloading files in the background.

Schedule a background URL session to download an item as shown below.

```
// Create a background session configuration.
let config = URLSessionConfiguration.background(withIdentifier: myRequestID)
config.isDiscretionary = true
config.sessionSendsLaunchEvents = true

// Create the background download task and schedule it to run in 15 minutes.
let urlSession = URLSession(configuration: config,
                            delegate: self,
                            delegateQueue: nil)

let backgroundTask = urlSession.downloadTask(with: url)
backgroundTask.earliestBeginDate = Date().addingTimeInterval(15 * 60)

// Run the task.
backgroundTask.resume()
```

If your app has a complication on the active watch face, it can receive up to four WKURLSessionRefreshBackgroundTask tasks per hour. To avoid throttling, use the earliestBeginDate property to schedule background URL session tasks no closer than 15 minutes apart.

Don’t subclass or create instances of this class. Instead, the system instantiates a WKURLSessionRefreshBackgroundTask object and passes the task object to your extension delegate’s handle(_:) method in response to URLSession events. Defer calling the background URLSession task’s `setTaskCompleted()` method until all the delegate method calls finish processing.

Note

In watchOS 9 and later, SwiftUI Background tasks are the preferred way to handle background tasks and interactions. For more information, backgroundTask(_:action:).

The system creates a background URLSession task when any of the following events occur:

- The server requires authentication to complete a background transfer.

- All background transfers associated with a session identifier complete (either successfully or unsuccessfully).

To get more information about the transfer, create a background configuration object with the same session identifier. Next, create a session object using the configuration object and a session delegate. The system automatically associates the new session with the transfer and calls the appropriate delegate methods.

## Topics

### Accessing background task data

var sessionIdentifier: String

The identifier for the triggering background transfer.

## Relationships

### Inherits From

- WKRefreshBackgroundTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Background tasks

Using background tasks

Handle scheduled update tasks in the background, and respond to background system interactions including Siri intents and incoming Bluetooth messages.

Preparing to take your watchOS app’s snapshot

Provide a timely, accurate snapshot of your app by using snapshot background tasks.

class WKApplicationRefreshBackgroundTask

A task that updates your app’s state in the background.

class WKWatchConnectivityRefreshBackgroundTask

A background task used to receive background updates from the Watch Connectivity framework.

class WKBluetoothAlertRefreshBackgroundTask

A task for handling timely Bluetooth alerts in the background.

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

