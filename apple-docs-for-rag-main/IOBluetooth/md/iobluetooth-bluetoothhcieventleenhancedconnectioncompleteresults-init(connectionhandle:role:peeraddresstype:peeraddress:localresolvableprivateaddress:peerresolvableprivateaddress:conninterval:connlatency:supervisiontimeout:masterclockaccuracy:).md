

- IOBluetooth
- BluetoothHCIEventLEEnhancedConnectionCompleteResults
-  init(connectionHandle:role:peerAddressType:peerAddress:localResolvablePrivateAddress:peerResolvablePrivateAddress:connInterval:connLatency:supervisionTimeout:masterClockAccuracy:) 

Initializer

# init(connectionHandle:role:peerAddressType:peerAddress:localResolvablePrivateAddress:peerResolvablePrivateAddress:connInterval:connLatency:supervisionTimeout:masterClockAccuracy:)

macOS

``` source
init(
    connectionHandle: BluetoothConnectionHandle,
    role: UInt8,
    peerAddressType: UInt8,
    peerAddress: BluetoothDeviceAddress,
    localResolvablePrivateAddress: BluetoothDeviceAddress,
    peerResolvablePrivateAddress: BluetoothDeviceAddress,
    connInterval: UInt16,
    connLatency: UInt16,
    supervisionTimeout: UInt16,
    masterClockAccuracy: UInt8
)
```

