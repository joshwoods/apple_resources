

- Watch Connectivity
-  WCSessionFile 

Class

# WCSessionFile

Information about a file currently being transferred between an iOS app and WatchKit extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
class WCSessionFile
```

## Overview

You do not create instances of this class directly. When you initiate a file transfer using the transferFile(_:metadata:) method of your app’s WCSession object, the session creates an instance when it queues the file for transfer. You can get a list of in-progress transfers initiated by your app from the session’s outstandingFileTransfers property. When a file is received by your app, the corresponding file object is delivered directly to your session’s delegate.

The file object includes the URL of the file on the local system and an optional dictionary of keys and values that accompany the file.

## Topics

### Getting the File Information

var fileURL: URL

The URL of the file that was received.

var metadata: [String : Any]?

A dictionary of additional information that was sent with the file.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Data Objects

class WCSessionFileTransfer

Information about in-progress file transfers.

class WCSessionUserInfoTransfer

Information about in-progress data transfers.

