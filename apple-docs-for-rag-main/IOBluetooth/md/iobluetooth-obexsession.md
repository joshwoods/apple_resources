

- IOBluetooth
-  OBEXSession 

Class

# OBEXSession

Object representing an OBEX connection to a remote target.

macOS

``` source
class OBEXSession
```

## Overview

You will have no need for a obtaining/using a raw OBEXSession, since it requires an underlying transport to do anything useful. However, once you have an object that is a subclass of this class, you can use the functions herein to manipulate that OBEXSession. First off, you will want to use OBEXConnect (if you are a client session) to actually cause the transport to open a connection to a remote target and establish an OBEX connection over it. From there you can issue more commands based on the responses from a server.

If you are a server session, the first thing you should receive is an OBEXConnect command packet, and you will want to issue an OBEXConnectResponse packet, with your reesponse to that command (success, denied, bad request, etc.).

You can use the session accessors to access certain information, such as the negotiated max packet length.

If you wish to implement your own OBEXSession over a transport such as ethernet, you will need to see the end of the file to determine which functions to override, and what to pass to those functions.

No timeout mechanism has been implemented so far for an OBEXSessions. If you need timeouts, you will need to implement them yourself. This is being explored for a future revision. However, be aware that the OBEX Specification does not explicitly require timeouts, so be sure you allow ample time for commands to complete, as some devices may be slow when sending large amounts of data.

## Topics

### DataTypes

struct OBEXTransportEvent

typealias OBEXTransportEventType

### Instance Methods

func clientHandleIncomingData(UnsafeMutablePointer&lt;OBEXTransportEvent>!)

Tranport subclasses need to invoke this from their own data-receive handlers. For example, when data is received over a Bluetooth RFCOMM channel in the IOBluetoothOBEXSession, it in turn calls this to dispatch the data. If you do not handle this case, your server session will not work, guaranteed.

func closeTransportConnection() -> OBEXError

You must override this - it will be called when the transport connection should be shutdown.

func getAvailableCommandPayloadLength(OBEXOpCode) -> OBEXMaxPacketLength

Determine the maximum amount of data you can send in a particular command as an OBEX client session.

func getAvailableCommandResponsePayloadLength(OBEXOpCode) -> OBEXMaxPacketLength

Determine the maximum amount of data you can send in a particular command response as an OBEX server session.

func getMaxPacketLength() -> OBEXMaxPacketLength

Gets current max packet length.

func hasOpenOBEXConnection() -> Bool

Has a successful connect packet been sent and received? This API tells you so.

func hasOpenTransportConnection() -> Bool

You must override this - it will be called periodically to determine if a transport connection is open or not.

func obexAbort(UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an OBEX Abort command to the session’s target.

func obexAbortResponse(OBEXOpCode, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an abort response to a session’s target.

func obexConnect(OBEXFlags, maxPacketLength: OBEXMaxPacketLength, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Initiate an OBEX connection to a device. Causes underlying transport (Bluetooth, et al) to attempt to connect to a remote device. After success, an OBEX connect packet is sent to establish the OBEX Connection.

func obexConnectResponse(OBEXOpCode, flags: OBEXFlags, maxPacketLength: OBEXMaxPacketLength, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send a connect response to a session’s target.

func obexDisconnect(UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an OBEX Disconnect command to the session’s target. THIS DOES NOT necessarily close the underlying transport connection. Deleting the session will ensure that closure.

func obexDisconnectResponse(OBEXOpCode, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send a disconnect response to a session’s target.

func obexGet(Bool, headers: UnsafeMutableRawPointer!, headersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an OBEX Get command to the session’s target.

func obexGetResponse(OBEXOpCode, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send a get response to a session’s target.

func obexPut(Bool, headersData: UnsafeMutableRawPointer!, headersDataLength: Int, bodyData: UnsafeMutableRawPointer!, bodyDataLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an OBEX Put command to the session’s target.

func obexPutResponse(OBEXOpCode, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send a put response to a session’s target.

func obexSetPath(OBEXFlags, constants: OBEXConstants, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send an OBEX SetPath command to the session’s target.

func obexSetPathResponse(OBEXOpCode, optionalHeaders: UnsafeMutableRawPointer!, optionalHeadersLength: Int, eventSelector: Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Send a set path response to a session’s target.

func openTransportConnection(Selector!, selectorTarget: Any!, refCon: UnsafeMutableRawPointer!) -> OBEXError

Opens a transport connection to a device. A Bluetooth connection is one example of a transport.

func sendData(toTransport: UnsafeMutableRawPointer!, dataLength: Int) -> OBEXError

You must override this to send data over your transport. This does nothing by default, it will return a kOBEXUnsupportedError.

func serverHandleIncomingData(UnsafeMutablePointer&lt;OBEXTransportEvent>!)

Tranport subclasses need to invoke this from their own data-receive handlers. For example, when data is received over a Bluetooth RFCOMM channel in the IOBluetoothOBEXSession, it in turn calls this to dispatch the data. If you do not handle this case, your server session will not work, guaranteed.

func setEventCallback(OBEXSessionEventCallback!)

Sets the C-API callback used when the session recieves data.

func setEventRefCon(UnsafeMutableRawPointer!)

Sets the C-API callback refCon used when the session recieves data.

func setEventSelector(Selector!, target: Any!, refCon: UnsafeMutableRawPointer!)

Allow you to set a selector to be called when events occur on the OBEX session.

## Relationships

### Inherits From

- NSObject

### Inherited By

- IOBluetoothOBEXSession

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

