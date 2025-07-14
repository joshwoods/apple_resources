

- Core WLAN
-  CWInterface 

Class

# CWInterface

Encapsulates an IEEE 802.11 interface.

macOS 10.6+

``` source
class CWInterface
```

## Overview

Provides access to various WLAN interface parameters, and operations such as scanning for networks, association, and creating computer-to-computer (ad-hoc) networks.

Important

Do not instantiate interface objects directly. Instead, use interface objects vended by a CWWiFiClient instance via the interface() method or one of its relatives. This enables your app to adopt App Sandbox even when it uses CoreWLAN without the need for any special exceptions. Directly instantiating interface objects causes low level access to system sockets, which by default is not allowed in a sandboxed environment.

## Topics

### Setting interface parameters

func setPairwiseMasterKey(Data?) throws

Sets the interface pairwise primary key (PMK).

func setPower(Bool) throws

Sets the interface power state.

func setWEPKey(Data?, flags: CWCipherKeyFlags, index: Int) throws

Sets the interface WEP key.

func setWLANChannel(CWChannel) throws

Sets the interface channel.

### Scanning for networks

func scanForNetworks(withName: String?) throws -> Set&lt;CWNetwork>

Scans for networks.

func scanForNetworks(withSSID: Data?) throws -> Set&lt;CWNetwork>

Scans for networks.

### Getting an interface

init(interfaceName: String?)

Convenience method for getting an CWInterface object with the specified name.

Deprecated

convenience init(name: String?)

An instance method for obtaining an CWInterface object.

Deprecated

### Getting all attached interfaces

class func interfaceNames() -> Set&lt;String>?

Returns the list of BSD names for WLAN interfaces available on the current system.

Deprecated

### Disassociating from a network

func disassociate()

Disassociates from the current network.

### Creating computer-to-computer networks

func startIBSSMode(withSSID: Data, security: CWIBSSModeSecurity, channel: Int, password: String?) throws

Creates a computer-to-computer (ad-hoc) network with the given network name, security type, and password on the specified channel.

Deprecated

### Committing a configuration

func commitConfiguration(CWConfiguration, authorization: SFAuthorization?) throws

Commit a configuration for the given WLAN interface.

### Associating to a network

func associate(toEnterpriseNetwork: CWNetwork, identity: SecIdentity?, username: String?, password: String?) throws

Connects to the given enterprise network.

func associate(to: CWNetwork, password: String?) throws

Associates to a given network using the given network passphrase.

### Instance Properties

var interfaceName: String?

The BSD name of the interface.

### Instance Methods

func activePHYMode() -> CWPHYMode

The current active PHY modes for the interface.

func bssid() -> String?

The current basic service set identifier (BSSID) for the interface, returned as a UTF-8 string.

func cachedScanResults() -> Set&lt;CWNetwork>?

The networks currently in the scan cache for the WLAN interface.

func configuration() -> CWConfiguration?

The current configuration for the given WLAN interface.

func countryCode() -> String?

The current country code (ISO/IEC 3166-1:1997) for the interface.

func hardwareAddress() -> String?

The hardware media access control (MAC) address for the interface, returned as a UTF-8 string.

func interfaceMode() -> CWInterfaceMode

The current mode for the interface.

func noiseMeasurement() -> Int

The current aggregate noise measurement (dBm) for the interface.

func powerOn() -> Bool

The interface power state is set to “ON”.

func rssiValue() -> Int

The current aggregate received signal strength indication (RSSI) measurement (dBm) for the interface.

func scanForNetworks(withName: String?, includeHidden: Bool) throws -> Set&lt;CWNetwork>

Scans for networks with the name you specify, optionally including hidden networks.

func scanForNetworks(withSSID: Data?, includeHidden: Bool) throws -> Set&lt;CWNetwork>

Scans for networks with the SSID you specify, optionally including hidden networks.

func security() -> CWSecurity

The current security mode for the interface.

func serviceActive() -> Bool

The interface has its corresponding network service enabled.

func ssid() -> String?

The current service set identifier (SSID) for the interface, encoded as a string.

func ssidData() -> Data?

The current service set identifier (SSID) for the interface, returned as data.

func supportedWLANChannels() -> Set&lt;CWChannel>?

An array of channels supported by the interface for the active country code.

func transmitPower() -> Int

The current transmit power (mW) for the interface.

func transmitRate() -> Double

The current transmit rate (Mbps) for the interface.

func wlanChannel() -> CWChannel?

The current channel for the interface.

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

class CWChannel

Encapsulates an IEEE 802.11 channel.

class CWConfiguration

Encapsulates an immutable configuration for an AirPort WLAN interface.

class CWMutableConfiguration

Encapsulates a mutable configuration for an AirPort WLAN interface.

class CWMutableNetworkProfile

Encapsulates a mutable network profile entry.

class CWNetwork

Encapsulates an IEEE 802.11 network, providing read-only accessors to various properties of the network.

class CWNetworkProfile

Encapsulates an immutable network profile entry.

class CWWiFiClient

A wrapper around the entire Wi-Fi subsystem that you use to access interfaces and set up event notifications.

