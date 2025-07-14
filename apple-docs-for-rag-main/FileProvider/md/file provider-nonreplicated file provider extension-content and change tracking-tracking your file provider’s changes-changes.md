

- File Provider
- Nonreplicated File Provider extension
- Content and Change Tracking
-  Tracking Your File Provider’s Changes 

# Tracking Your File Provider’s Changes

Create an enumerator to track changes to your file provider’s content.

## Overview

While an enumerator is active, it also tracks any changes to its contents. The system only tracks changes to a document or folder while it has an active enumerator for that item (for example, while a document is open or a folder is being browsed).

Note

The system always tracks changes to the working set. If it doesn’t have an active enumerator for the working set, it creates a new one.

When your file provider app or extension identifies a change to its content:

- Call the NSFileProviderManager class’s signalEnumerator(for:completionHandler:) method to notify the system of the change. Pass the item’s identifier as the `containerItemIdentifier` property.

- If the change affects the working set, call signalEnumerator(for:completionHandler:) a second time. Pass the workingSet constant as the `containerItemIdentifier` property. This tells the system to update the working set.

After the system is alerted to the change, it calls enumerateChanges(for:from:) on any affected, active enumerations and updates the browser’s user interface as needed. This method is asynchronous. When it’s called, the enumerator gathers information about the items (perhaps from a remote server) in the background, and returns the results to the specified observer (an object that adopts the NSFileProviderChangeObserver protocol).

## Topics

### Tracking Document Changes

Tracking Changes to Documents

Track and report changes to open documents.

### Signaling Changes with Push Notifications

Using push notifications to signal changes

Send push notifications to a device to signal changes from your server.

## See Also

### Change Tracking

protocol NSFileProviderChangeObserver

An observer that receives changes and deletions during enumeration.

struct NSFileProviderSyncAnchor

A synchronization point that represents the last batch of changes returned by the enumerator.

