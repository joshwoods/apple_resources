

- File Provider
- NSFileProviderManager
- NSFileProviderManager.DisconnectionOptions
-  temporary 

Type Property

# temporary

A temporary disconnection.

macOS 11.0+

``` source
static var temporary: NSFileProviderManager.DisconnectionOptions { get }
```

## Discussion

Include the temporary value when the disconnection is temporary, such as when updating the domain. Exclude this value when the disconnection isn’t temporary, like when the user logs out.

