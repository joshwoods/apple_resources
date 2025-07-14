

- Network Extension
- NEProvider
-  defaultPath Deprecated

Instance Property

# defaultPath

The current default network path used for connections created by the provider.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var defaultPath: NWPath? { get }
```

Deprecated

Use the nw_path_monitor_t type from the Network framework instead.

## Discussion

This NWPath object contains information about which physical network interface will be used by connections opened by the Network Extension provider. You can determine when this physical interface changes by observing this property using KVO.

