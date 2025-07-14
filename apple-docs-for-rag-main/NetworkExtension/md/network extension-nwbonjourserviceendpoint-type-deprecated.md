

- Network Extension
- NWBonjourServiceEndpoint
-  type Deprecated

Instance Property

# type

The endpoint’s Bonjour service type.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var type: String { get }
```

Deprecated

Use the nw_endpoint_get_bonjour_service_type(_:) function from the Network framework instead.

## Discussion

For example, the service type could be `"_music._tcp"`.

## See Also

### Getting endpoint properties

var name: String

The endpoint’s Bonjour service name.

Deprecated

var domain: String

The endpoint’s Bonjour service domain, such as `"local"`.

Deprecated

