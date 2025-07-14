

- SwiftUI
-  BackgroundTask 

Structure

# BackgroundTask

The kinds of background tasks that your app or extension can handle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct BackgroundTask
```

## Overview

Use a value of this type with the backgroundTask(_:action:) scene modifier to create a handler for background tasks that the system sends to your app or extension. For example, you can use urlSession to define an asynchronous closure that the system calls when it launches your app or extension to handle a response from a background URLSession.

## Topics

### Refreshing the app

static var appRefresh: BackgroundTask&lt;String?, Void>

A task that updates your app’s state in the background.

static func appRefresh(String) -> BackgroundTask&lt;Void, Void>

A task that updates your app’s state in the background for a matching identifier.

### Preparing for a snapshot

static var snapshot: BackgroundTask&lt;SnapshotData, SnapshotResponse>

A background task used to update your app’s user interface in preparation for a snapshot.

### Receiving connectivity updates

static var bluetoothAlert: BackgroundTask&lt;Void, Void>

A background task used to receive critical alerts from paired bluetooth accessories.

static var watchConnectivity: BackgroundTask&lt;Void, Void>

A background task used to receive background updates from the Watch Connectivity framework.

### Responding to URL sessions

static var urlSession: BackgroundTask&lt;String, Void>

A task that responds to background URL sessions.

static func urlSession(String) -> BackgroundTask&lt;Void, Void>

A task that responds to background URL sessions matching the given identifier.

static func urlSession(matching: (String) -> Bool) -> BackgroundTask&lt;String, Void>

A task that responds to background URL sessions matching the given predicate.

### Updating intents and shortcuts

static var intentDidRun: BackgroundTask&lt;Void, Void>

A background task used to update your app after a SiriKit intent runs.

static var relevantShortcut: BackgroundTask&lt;Void, Void>

A background task used to periodically donate relevant Siri shortcuts.

## Relationships

### Conforms To

- Sendable

## See Also

### Handling background tasks

func backgroundTask&lt;D, R>(BackgroundTask&lt;D, R>, action: (D) async -> R) -> some Scene

Runs the specified action when the system provides a background task.

struct SnapshotData

The associated data of a snapshot background task.

struct SnapshotResponse

Your appplication’s response to a snapshot background task.

