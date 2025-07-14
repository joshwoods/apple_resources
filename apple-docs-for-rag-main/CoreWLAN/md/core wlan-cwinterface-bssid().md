

- Core WLAN
- CWInterface
-  bssid() 

Instance Method

# bssid()

The current basic service set identifier (BSSID) for the interface, returned as a UTF-8 string.

macOS 10.6+

``` source
func bssid() -> String?
```

## Discussion

Dynamically queries the interface for the current BSSID. Returns a UTF-8 string formatted as \, or *nil* in the case of an error, or if the interface is not participating in a network.

## See Also

### Instance Methods

func activePHYMode() -> CWPHYMode

The current active PHY modes for the interface.

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

