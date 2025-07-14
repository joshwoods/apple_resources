

- Core WLAN
- CWInterface
-  associate(toEnterpriseNetwork:identity:username:password:) 

Instance Method

# associate(toEnterpriseNetwork:identity:username:password:)

Connects to the given enterprise network.

macOS 10.7+

``` source
func associate(
    toEnterpriseNetwork network: CWNetwork,
    identity: SecIdentity?,
    username: String?,
    password: String?
) throws
```

## Parameters 

`network`  

The network to which the interface will associate.

`identity`  

The identity to use for IEEE 802.1X authentication. Holds the corresponding client certificate.

`username`  

The username to use for IEEE 802.1X authentication.

`password`  

The password to use for IEEE 802.1X authentication.

## Discussion

This method will block for the duration of the association. This operation may require an administrator password.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Associating to a network

func associate(to: CWNetwork, password: String?) throws

Associates to a given network using the given network passphrase.

