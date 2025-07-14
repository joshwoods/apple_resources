

- Authentication Services
- ASAuthorizationProviderExtensionKerberosMapping
-  encryptionKeyTypeKeyName 

Instance Property

# encryptionKeyTypeKeyName

The key name of the Kerberos session key type number.

macOS 13.0+

``` source
var encryptionKeyTypeKeyName: String? { get set }
```

## Discussion

Ensure the value for this key is the correct encryption type for the session key. See section 7 of RFC 3962 for more information.

## See Also

### Getting the properties

var clientNameKeyName: String?

The key name of the Kerberos client name string.

var messageBufferKeyName: String?

The key name of the Base 64-encoded Kerberos AS-REP string.

var realmKeyName: String?

The key name of the Kerberos realm string.

var serviceNameKeyName: String?

The key name of the Kerberos service name string.

var sessionKeyKeyName: String?

The key name of the Kerberos session key.

var ticketKeyPath: String?

The keypath in the response JSON that uses this set of mappings.

