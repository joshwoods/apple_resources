

- SMS and Call Reporting
- ILMessageFilterError
-  redundantNetworkDeferral 

Type Property

# redundantNetworkDeferral

The app extension tried to defer a request to its network service more than once, which isn’t allowed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
static var redundantNetworkDeferral: ILMessageFilterError.Code { get }
```

## See Also

### Error Codes

static var invalidNetworkURL: ILMessageFilterError.Code

The network request URL given by the `ILMessageFilterExtensionNetworkURL` key in the app extension’s information property list file is either missing or invalid.

static var networkRequestFailed: ILMessageFilterError.Code

The network request failed.

static var networkURLUnauthorized: ILMessageFilterError.Code

The app extension’s containing app isn’t authorized to allow the app extension to defer network requests to the host specified in its information property list file.

static var system: ILMessageFilterError.Code

An unspecified system error occurred.

