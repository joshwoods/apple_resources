

- Core Location
- CLBeaconRegion
-  peripheralData(withMeasuredPower:) 

Instance Method

# peripheralData(withMeasuredPower:)

Retrieves data that you can use to advertise the current device as a beacon.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
func peripheralData(withMeasuredPower measuredPower: NSNumber?) -> NSMutableDictionary
```

## Parameters 

`measuredPower`  

The received signal strength indicator (RSSI) value, measured in decibels, for the device. This value represents the measured strength of the beacon from one meter away that Core Location uses during ranging. Specify `nil` to use the default value for the device.

## Return Value

A dictionary of data that you can use in conjunction with a CBPeripheralManager to advertise the current device as a beacon.

## Mentioned in 

Turning an iOS device into an iBeacon device

## Discussion

The returned dictionary encodes the beacon’s identifying information, along with other information needed to advertise the beacon. You don’t need to access the dictionary contents directly. Pass the dictionary to the startAdvertising(_:) method of a CBPeripheralManager to begin advertising the beacon.

