

- Authentication Services
- ASAuthorizationProviderExtensionKerberosMapping
-  ticketKeyPath 

Instance Property

# ticketKeyPath

The keypath in the response JSON that uses this set of mappings.

macOS 13.0+

``` source
var ticketKeyPath: String? { get set }
```

## Discussion

If the response tokens from the login contain this keypath, the system uses this mapping to create a Kerberos ticket. The expected response is a JSON dictionary with the supplied key names containing Kerberos ticket values.

## See Also

### Getting the properties

var clientNameKeyName: String?

The key name of the Kerberos client name string.

var encryptionKeyTypeKeyName: String?

The key name of the Kerberos session key type number.

var messageBufferKeyName: String?

The key name of the Base 64-encoded Kerberos AS-REP string.

var realmKeyName: String?

The key name of the Kerberos realm string.

var serviceNameKeyName: String?

The key name of the Kerberos service name string.

var sessionKeyKeyName: String?

The key name of the Kerberos session key.

