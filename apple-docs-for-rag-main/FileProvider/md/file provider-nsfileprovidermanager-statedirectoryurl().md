

- File Provider
- NSFileProviderManager
-  stateDirectoryURL() 

Instance Method

# stateDirectoryURL()

Returns a URL for a directory for storing state information for the domain.

macOS 15.0+

``` source
func stateDirectoryURL() throws -> URL
```

## See Also

### Working with external volumes

class func checkDomainsCanBeStoredOnVolume(at: URL) throws -> NSFileProviderManager.EligibilityResult

Checks whether the specified URL is eligible for storing a domain.

enum EligibilityResult

Constants that specify whether a URL is eligible for storing a domain.

protocol NSFileProviderExternalVolumeHandling

A protocol that defines the interface for handling external volumes.

