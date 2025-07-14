

- Core Services
-  File System Events 

API Collection

# File System Events

Get notifications when the contents of a directory hierarchy change.

## Overview

The file system events API provides a way for your application to ask for notification when the contents of a directory hierarchy are modified. For example, your application can use this to quickly detect when the user modifies a file within a project bundle using another application.

It also provides a lightweight way to determine whether the contents of a directory hierarchy have changed since your application last examined them. For example, a backup application can use this to determine what files have changed since a given time stamp or a given event ID.

## Topics

### Functions

func FSEventStreamCopyDescription(ConstFSEventStreamRef) -> CFString

func FSEventStreamCopyPathsBeingWatched(ConstFSEventStreamRef) -> CFArray

func FSEventStreamCreate(CFAllocator?, FSEventStreamCallback, UnsafeMutablePointer&lt;FSEventStreamContext>?, CFArray, FSEventStreamEventId, CFTimeInterval, FSEventStreamCreateFlags) -> FSEventStreamRef?

func FSEventStreamCreateRelativeToDevice(CFAllocator?, FSEventStreamCallback, UnsafeMutablePointer&lt;FSEventStreamContext>?, dev_t, CFArray, FSEventStreamEventId, CFTimeInterval, FSEventStreamCreateFlags) -> FSEventStreamRef?

func FSEventStreamFlushAsync(FSEventStreamRef) -> FSEventStreamEventId

func FSEventStreamFlushSync(FSEventStreamRef)

func FSEventStreamGetDeviceBeingWatched(ConstFSEventStreamRef) -> dev_t

func FSEventStreamGetLatestEventId(ConstFSEventStreamRef) -> FSEventStreamEventId

func FSEventStreamInvalidate(FSEventStreamRef)

func FSEventStreamRelease(FSEventStreamRef)

func FSEventStreamRetain(FSEventStreamRef)

func FSEventStreamScheduleWithRunLoop(FSEventStreamRef, CFRunLoop, CFString)Deprecated

func FSEventStreamSetDispatchQueue(FSEventStreamRef, dispatch_queue_t?)

Schedules the stream on the specified dispatch queue.

func FSEventStreamSetExclusionPaths(FSEventStreamRef, CFArray) -> Bool

func FSEventStreamShow(ConstFSEventStreamRef)

func FSEventStreamStart(FSEventStreamRef) -> Bool

func FSEventStreamStop(FSEventStreamRef)

func FSEventStreamUnscheduleFromRunLoop(FSEventStreamRef, CFRunLoop, CFString)Deprecated

func FSEventsCopyUUIDForDevice(dev_t) -> CFUUID?

func FSEventsGetCurrentEventId() -> FSEventStreamEventId

func FSEventsGetLastEventIdForDeviceBeforeTime(dev_t, CFAbsoluteTime) -> FSEventStreamEventId

func FSEventsPurgeEventsForDeviceUpToEventId(dev_t, FSEventStreamEventId) -> Bool

### Enumerations

FSEventStreamCreateFlags

FSEventStreamEventFlags

### Data Types

typealias FSEventStreamCallback

typealias FSEventStreamCreateFlags

typealias FSEventStreamEventFlags

typealias FSEventStreamEventId

typealias FSEventStreamRef

### Constants

var kFSEventStreamEventExtendedDataPathKey: String

var kFSEventStreamEventExtendedFileIDKey: String

## See Also

### Related Documentation

File System Events Programming Guide

