

- File Provider
- NSFileProviderManager
-  checkDomainsCanBeStoredOnVolume(at:) 

Type Method

# checkDomainsCanBeStoredOnVolume(at:)

Checks whether the specified URL is eligible for storing a domain.

macOS 15.0+

``` source
class func checkDomainsCanBeStoredOnVolume(at url: URL) throws -> NSFileProviderManager.EligibilityResult
```

## See Also

### Working with external volumes

func stateDirectoryURL() throws -> URL

Returns a URL for a directory for storing state information for the domain.

enum EligibilityResult

Constants that specify whether a URL is eligible for storing a domain.

protocol NSFileProviderExternalVolumeHandling

A protocol that defines the interface for handling external volumes.

