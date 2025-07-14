

- PassKit (Apple Pay and Wallet)
- PKPass
-  authenticationToken 

Instance Property

# authenticationToken

The token for authenticating update requests.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var authenticationToken: String? { get }
```

## Discussion

Use this property to store an authentication token for your web service. When the device requests an updated copy of the pass, the request’s header includes this authorization token. Use this token to verify that the request is from a valid device and not from an unauthorized source.

Don’t change the authentication token during an update.

## See Also

### Getting the web service information

var webServiceURL: URL?

The URL for the web service.

