

- Device Management
-  AppManagedAttributesObject 

Object

# AppManagedAttributesObject

A dictionary of values associated with an app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object AppManagedAttributesObject
```

## Properties

`AssociatedDomains`

`[string]`

An array of domain names to associate with the app.

`AssociatedDomainsEnableDirectDownloads`

`boolean`

If `true`, the system enables direct downloads for the `AssociatedDomains`.

Default: `false`

`CellularSliceUUID`

`string`

The cellular slice identifier, which can be the data network name (DNN) or app category. For DNN, encode the value as “DNN:name”, where “name” is the carrier-provided DNN name. For app category, encode the value as “AppCategory:category”, where “category” is a carrier-provided string such as “Enterprise1”.

`ContentFilterUUID`

`string`

The UUID of the content filter to associate with the app.

`DNSProxyUUID`

`string`

The UUID of the DNS proxy to associate with the app.

`RelayUUID`

`string`

The UUID of the relay to associate with the app.

`TapToPayScreenLock`

`boolean`

If `true`, the device automatically locks after every transaction that requires a customer’s card PIN. If `false`, the user can choose the behavior.

Default: `false`

`VPNUUID`

`string`

The UUID of the VPN to associate with the app.

## See Also

### Objects

object AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

object AppManagedCredentialConfigObject

A dictionary of values associated with a credential config.

object AppManagedExtensionConfigsObject

A dictionary of values associated with an extension config.

object AppManagedInstallBehaviorObject

A dictionary that describes how and when to install an app.

