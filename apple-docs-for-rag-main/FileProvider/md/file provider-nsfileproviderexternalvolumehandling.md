

- File Provider
-  NSFileProviderExternalVolumeHandling 

Protocol

# NSFileProviderExternalVolumeHandling

A protocol that defines the interface for handling external volumes.

macOS 15.0+

``` source
protocol NSFileProviderExternalVolumeHandling : NSObjectProtocol
```

## Topics

### Connecting to external domains

func shouldConnectExternalDomain(completionHandler: ((any Error)?) -> Void)

Determines whether to connect to a domain from another device.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with external volumes

func stateDirectoryURL() throws -> URL

Returns a URL for a directory for storing state information for the domain.

class func checkDomainsCanBeStoredOnVolume(at: URL) throws -> NSFileProviderManager.EligibilityResult

Checks whether the specified URL is eligible for storing a domain.

enum EligibilityResult

Constants that specify whether a URL is eligible for storing a domain.

