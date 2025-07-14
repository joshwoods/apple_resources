

- CloudKit
-  CKSyncEngineDelegate 

Protocol

# CKSyncEngineDelegate

An interface for providing record data to a sync engine and customizing that engine’s behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
protocol CKSyncEngineDelegate : AnyObject, Sendable
```

## Overview

Important

CKSyncEngine delivers events serially, which means the delegate doesn’t receive the next event until it finishes handling the current one. To maintain this ordering, don’t call sync engine methods from your delegate that may cause the engine to generate additional events. For example, don’t invoke fetchChanges(_:) or sendChanges(_:) from within handleEvent(_:syncEngine:).

## Topics

### Handling sync events

func handleEvent(CKSyncEngine.Event, syncEngine: CKSyncEngine) async

Tells the delegate to handle the specified sync event.

**Required**

enum Event

Describes an event that occurs during a sync operation.

enum CKSyncEngineEventType

Describes an event that occurs during a sync operation.

### Sending changes

func nextRecordZoneChangeBatch(CKSyncEngine.SendChangesContext, syncEngine: CKSyncEngine) async -> CKSyncEngine.RecordZoneChangeBatch?

Asks the delegate to provide the next set of record changes to send to the server.

**Required**

struct SendChangesContext

A type that describes a single attempt to send changes to the iCloud servers.

struct RecordZoneChangeBatch

A type that contains the record changes for a single send operation.

### Instance Methods

func nextFetchChangesOptions(CKSyncEngine.FetchChangesContext, syncEngine: CKSyncEngine) async -> CKSyncEngine.FetchChangesOptions

**Required** Default implementation provided.

## Relationships

### Inherits From

- Sendable

