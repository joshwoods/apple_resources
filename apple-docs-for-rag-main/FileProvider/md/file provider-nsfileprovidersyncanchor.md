

- File Provider
-  NSFileProviderSyncAnchor 

Structure

# NSFileProviderSyncAnchor

A synchronization point that represents the last batch of changes returned by the enumerator.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderSyncAnchor
```

## Discussion

Your file provider should populate the sync anchor with the information it needs to identify and enumerate only the changes that occurred after the synchronization point. For example, a simple sync anchor could use the time and date of the last update successfully downloaded from the server. A request to enumerate changes from that sync anchor would then return only the changes downloaded after that date.

The system only retains the last anchor passed to it. After the system calls enumerateChanges(for:from:) with a sync anchor, it’s safe to deallocate any older sync anchors.

## Topics

### Creating Sync Anchors

init(Data)

Returns a new sync anchor.

init(rawValue: Data)

Returns a new sync anchor from the provided data object.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Change Tracking

Tracking Your File Provider’s Changes

Create an enumerator to track changes to your file provider’s content.

protocol NSFileProviderChangeObserver

An observer that receives changes and deletions during enumeration.

