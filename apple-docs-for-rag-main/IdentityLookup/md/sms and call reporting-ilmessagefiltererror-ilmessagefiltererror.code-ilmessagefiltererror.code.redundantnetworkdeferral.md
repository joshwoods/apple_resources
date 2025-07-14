

- SMS and Call Reporting
- ILMessageFilterError
- ILMessageFilterError.Code
-  ILMessageFilterError.Code.redundantNetworkDeferral 

Case

# ILMessageFilterError.Code.redundantNetworkDeferral

The app extension tried to defer a request to its network service more than once, which isn’t allowed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
case redundantNetworkDeferral
```

## See Also

### Error Codes

case system

An unspecified system error occurred.

case invalidNetworkURL

The network request URL given by the `ILMessageFilterExtensionNetworkURL` key in the app extension’s `Info.plist` file is either missing or invalid.

case networkURLUnauthorized

The app extension’s containing app isn’t authorized to allow the app extension to defer network requests to the host specified in its `Info.plist` file.

case networkRequestFailed

The network request failed.

