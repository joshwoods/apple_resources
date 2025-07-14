

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  SMS Dictionary Key Constants 

API Collection

# SMS Dictionary Key Constants

Read the parts of an SMS message.

## Topics

### Sender Information

let IOBluetoothPDUOriginatingAddress: String

The phone number for the sender of the text message.

let IOBluetoothPDUOriginatingAddressType: String

The format of the phone number for the sender of the text message.

let IOBluetoothPDUServicCenterAddress: String

The phone number for the service center that stored and then delivered the message.

let IOBluetoothPDUServiceCenterAddressType: String

The format of the phone number for the service center.

### Message Information

let IOBluetoothPDUProtocolID: String

The protocol of the text message content.

let IOBluetoothPDUUserData: String

The content of the text message.

let IOBluetoothPDUTimestamp: String

The time the text message was sent.

let IOBluetoothPDUType: String

The GSM type of the text message.

let IOBluetoothPDUEncoding: String

The encoding for the text message.

## See Also

### Receiving SMS Information

func handsFree(IOBluetoothHandsFreeDevice!, incomingSMS: [AnyHashable : Any]!)

Tells the delegate there’s an incoming text message.

