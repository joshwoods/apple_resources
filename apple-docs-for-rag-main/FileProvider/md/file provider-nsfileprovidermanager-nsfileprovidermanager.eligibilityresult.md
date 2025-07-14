

- File Provider
- NSFileProviderManager
-  NSFileProviderManager.EligibilityResult 

Enumeration

# NSFileProviderManager.EligibilityResult

Constants that specify whether a URL is eligible for storing a domain.

macOS 15.0+

``` source
enum EligibilityResult
```

## Topics

### Determining eligibility

case eligible

case ineligible(NSFileProviderVolumeUnsupportedReason)

struct NSFileProviderVolumeUnsupportedReason

Constants that describe why an external volume might not be eligible for storing a domain.

## Relationships

### Conforms To

- Equatable

## See Also

### Working with external volumes

func stateDirectoryURL() throws -> URL

Returns a URL for a directory for storing state information for the domain.

class func checkDomainsCanBeStoredOnVolume(at: URL) throws -> NSFileProviderManager.EligibilityResult

Checks whether the specified URL is eligible for storing a domain.

protocol NSFileProviderExternalVolumeHandling

A protocol that defines the interface for handling external volumes.

