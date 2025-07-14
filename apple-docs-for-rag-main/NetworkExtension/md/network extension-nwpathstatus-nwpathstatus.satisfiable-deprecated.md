

- Network Extension
- NWPathStatus
-  NWPathStatus.satisfiable Deprecated

Case

# NWPathStatus.satisfiable

The path is not currently satisfied, but may become satisfied upon a connection attempt. This can be due to a service, such as a VPN or a cellular data connection not being activated.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
case satisfiable
```

Deprecated

Use the nw_path_status_t type from the Network framework instead.

## See Also

### Path Statuses

case invalid

The path cannot be evaluated.

Deprecated

case satisfied

The path is ready to be used for network connections.

Deprecated

case unsatisfied

The path for network connections is not available, either due to lack of network connectivity or being prohibited by system policy.

Deprecated

