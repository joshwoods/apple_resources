

- Watch Connectivity
-  WCSessionFileTransfer 

Class

# WCSessionFileTransfer

Information about in-progress file transfers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
class WCSessionFileTransfer
```

## Overview

You do not create instances of this class yourself. When you initiate a file transfer, the system creates a new file transfer object to represent the transferred file. Use that object to get the file information or to cancel the transfer as needed.

To initiate a file transfer operation, call the transferFile(_:metadata:) method of your app’s WCSession object.

## Topics

### Getting the File Information

var file: WCSessionFile

The file being transferred.

### Managing the File Transfer

var isTransferring: Bool

A Boolean value indicating whether the file is still being transferred.

var progress: Progress

An object that tracks the progress of the file transfer.

func cancel()

Cancels the file transfer.

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

class WCSessionFile

Information about a file currently being transferred between an iOS app and WatchKit extension.

class WCSessionUserInfoTransfer

Information about in-progress data transfers.

