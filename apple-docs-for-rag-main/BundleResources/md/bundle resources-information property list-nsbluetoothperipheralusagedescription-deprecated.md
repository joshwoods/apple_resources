

- Bundle Resources
- Information Property List
-  NSBluetoothPeripheralUsageDescription Deprecated

Property List Key

# NSBluetoothPeripheralUsageDescription

A message that tells the user why the app is requesting the ability to connect to Bluetooth peripherals.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0Deprecated

## Details 

Name  
Privacy - Bluetooth Peripheral Usage Description

Type  

string

## Discussion

For apps with a deployment target of iOS 13 and later, use NSBluetoothAlwaysUsageDescription instead.

For deployment targets earlier than iOS 13, add both NSBluetoothAlwaysUsageDescription and NSBluetoothPeripheralUsageDescription to your app’s Information Property List file. Devices running earlier versions of iOS rely on NSBluetoothPeripheralUsageDescription, while devices running later versions rely on NSBluetoothAlwaysUsageDescription.

Important

This key is required if your app uses APIs that access Bluetooth peripherals and has a deployment target earlier than iOS 13.

## See Also

### Bluetooth

NSBluetoothAlwaysUsageDescription

A message that tells the user why the app needs access to Bluetooth.

**Name:** Privacy - Bluetooth Always Usage Description

