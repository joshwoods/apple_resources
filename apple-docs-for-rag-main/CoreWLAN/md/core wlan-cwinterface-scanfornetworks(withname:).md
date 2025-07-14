

- Core WLAN
- CWInterface
-  scanForNetworks(withName:) 

Instance Method

# scanForNetworks(withName:)

Scans for networks.

macOS 10.7+

``` source
func scanForNetworks(withName networkName: String?) throws -> Set
```

## Parameters 

`networkName`  

The name (SSID) of the network for which to scan.

## Return Value

A set of CWNetwork objects.

## Discussion

If *ssid* parameter is present, a directed scan will be performed by the interface, otherwise a broadcast scan will be performed. This method will block for the duration of the scan.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Scanning for networks

func scanForNetworks(withSSID: Data?) throws -> Set&lt;CWNetwork>

Scans for networks.

