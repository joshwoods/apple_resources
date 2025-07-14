

- IOBluetooth
-  IOBluetoothDeviceSearchAttributes 

Structure

# IOBluetoothDeviceSearchAttributes

Structure used to search for particular devices.

macOS

``` source
struct IOBluetoothDeviceSearchAttributes
```

## Overview

You can search for general device classes and service classes, or you can search for a specific device address or name. If you pass NULL as the attribute structure, you will get ALL devices in the vicinity found during a search. Note that passing a zeroed out block of attributes is NOT equivalent to passing in NULL!

## Topics

### Initializers

init()

init(options: IOBluetoothDeviceSearchOptions, maxResults: IOItemCount, deviceAttributeCount: IOItemCount, attributeList: UnsafeMutablePointer&lt;IOBluetoothDeviceSearchDeviceAttributes>!)

### Instance Properties

var attributeList: UnsafeMutablePointer&lt;IOBluetoothDeviceSearchDeviceAttributes>!

var deviceAttributeCount: IOItemCount

var maxResults: IOItemCount

var options: IOBluetoothDeviceSearchOptions

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct BluetoothAFHHostChannelClassification

struct BluetoothAFHResults

struct BluetoothAMPCommandRejectReason

struct BluetoothAMPCreatePhysicalLinkResponseStatus

struct BluetoothAMPDisconnectPhysicalLinkResponseStatus

struct BluetoothAMPDiscoverResponseControllerStatus

struct BluetoothAMPGetAssocResponseStatus

struct BluetoothAMPGetInfoResponseStatus

struct BluetoothAMPManagerCode

struct BluetoothAuthenticationRequirementsValues

struct BluetoothCompanyIdentifers

struct BluetoothDeviceAddress

struct BluetoothEnhancedSynchronousConnectionInfo

struct BluetoothEventFilterCondition

struct BluetoothFeatureBits

