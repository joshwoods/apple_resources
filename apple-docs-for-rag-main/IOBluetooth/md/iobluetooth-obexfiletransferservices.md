

- IOBluetooth
-  OBEXFileTransferServices 

Class

# OBEXFileTransferServices

Implements advanced OBEX operations in addition to simple PUT and GET.

macOS

``` source
class OBEXFileTransferServices
```

## Overview

All operations are asynchronous and will callback over a respective delegate method if the initial return value is successful. The initial return value usually concerns the state of this object where as the delegate return value reflects the response of the remote device.

## Topics

### Initializers

init!(obexSession: IOBluetoothOBEXSession!)

Create a new OBEXFileTransferServices object

### Instance Properties

var delegate: AnyObject!

### Instance Methods

func abort() -> OBEXError

Abort the current operation

func changeCurrentFolderBackward() -> OBEXError

Change to the directory above the current level if not at the root

func changeCurrentFolderForward(toPath: String!) -> OBEXError

Change the remote path

func changeCurrentFolderToRoot() -> OBEXError

Asynchronously change to the remote root directory

func connectToFTPService() -> OBEXError

Connect to a remote device for FTP operations

func connectToObjectPushService() -> OBEXError

Connect to a remote device for ObjectPush operations. Most of the FTP functionality of this object will be disabled.

func copyRemoteFile(String!, toLocalPath: String!) -> OBEXError

Copy a remote file to a local path

func createFolder(String!) -> OBEXError

Create a folder on the remote target

func currentPath() -> String!

Get the remote current directory path during an FTP session

func disconnect() -> OBEXError

Disconnect from the remote device

func getDefaultVCard(String!) -> OBEXError

Get the remote default VCard, if it is supported

func isBusy() -> Bool

Get the action state of the module

func isConnected() -> Bool

Get the connected state of this module.

func removeItem(String!) -> OBEXError

Remove a remote item.

func retrieveFolderListing() -> OBEXError

Get a remote directory listing

func send(Data!, type: String!, name: String!) -> OBEXError

Send data to a remote target

func sendFile(String!) -> OBEXError

Put a local file to the remote target

### Type Methods

class func withOBEXSession(IOBluetoothOBEXSession!) -> Self!

Create a new OBEXFileTransferServices object

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

### Classes

class IOBluetoothDevice

An instance of IOBluetoothDevice represents a single remote Bluetooth device.

class IOBluetoothDeviceInquiry

Object representing a device inquiry that finds Bluetooth devices in-range of the computer, and (optionally) retrieves name information for them.

class IOBluetoothDevicePair

An instance of IOBluetoothDevicePair represents a pairing attempt to a remote Bluetooth device.

class IOBluetoothDeviceRef

An object that represents a Bluetooth I/O device.

class IOBluetoothHandsFree

Hands free profile class.

class IOBluetoothHandsFreeAudioGateway

An object that sends data to a connected Bluetooth hands-free phone or headset and processes commands from it.

class IOBluetoothHandsFreeDevice

An object you use to manage phone calls on a connected Bluetooth hands-free phone or headset.

class IOBluetoothHostController

This class is a representation of a Bluetooth Host Controller Interface that is present on the local computer (either plugged in externally or available internally).

class IOBluetoothL2CAPChannel

An instance of IOBluetoothL2CAPChannel represents a single open L2CAP channel.

class IOBluetoothL2CAPChannelRef

class IOBluetoothOBEXSession

An OBEX Session with a Bluetooth RFCOMM channel as the transport.

class IOBluetoothObject

class IOBluetoothObjectRef

class IOBluetoothRFCOMMChannel

An instance of this class represents an RFCOMM channel as defined by the Bluetooth SDP spec..

class IOBluetoothRFCOMMChannelRef

