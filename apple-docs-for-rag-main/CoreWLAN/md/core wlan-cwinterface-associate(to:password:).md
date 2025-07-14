

- Core WLAN
- CWInterface
-  associate(to:password:) 

Instance Method

# associate(to:password:)

Associates to a given network using the given network passphrase.

macOS 10.7+

``` source
func associate(
    to network: CWNetwork,
    password: String?
) throws
```

## Parameters 

`network`  

The network to which the interface will associate.

`password`  

The network passphrase or key. Required for association to WEP, WPA Personal, and WPA2 Personal networks.

## Discussion

This method will block for the duration of the association. This operation may require an administrator password.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Associating to a network

func associate(toEnterpriseNetwork: CWNetwork, identity: SecIdentity?, username: String?, password: String?) throws

Connects to the given enterprise network.

