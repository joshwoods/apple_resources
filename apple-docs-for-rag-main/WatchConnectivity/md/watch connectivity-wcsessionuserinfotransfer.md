

- Watch Connectivity
-  WCSessionUserInfoTransfer 

Class

# WCSessionUserInfoTransfer

Information about in-progress data transfers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
class WCSessionUserInfoTransfer
```

## Overview

You don’t create instances of this class yourself. When you begin a data transfer, the system creates a new instance of this class for you. Use the created object to monitor or cancel the transfer as needed.

To initiate a file transfer operation, call the transferUserInfo(_:) or transferCurrentComplicationUserInfo(_:) method of your app’s WCSession object.

## Topics

### Getting the Transfer Information

var isCurrentComplicationInfo: Bool

A Boolean indicating whether the data is related to the app’s complication.

var userInfo: [String : Any]

The data being transferred.

### Managing the Transfer Operation

var isTransferring: Bool

A Boolean value indicating whether the data is still being transferred.

func cancel()

Cancels the data transfer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Data Objects

class WCSessionFile

Information about a file currently being transferred between an iOS app and WatchKit extension.

class WCSessionFileTransfer

Information about in-progress file transfers.

