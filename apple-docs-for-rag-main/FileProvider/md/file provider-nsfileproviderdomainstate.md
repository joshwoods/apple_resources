

- File Provider
-  NSFileProviderDomainState 

Protocol

# NSFileProviderDomainState

An object that contains global state data about the domain.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
protocol NSFileProviderDomainState : NSObjectProtocol
```

## Topics

### Accessing State Data

var domainVersion: NSFileProviderDomainVersion

An opaque object that uniquely identifies the domain’s version.

**Required**

var userInfo: [AnyHashable : Any]

Global state information about the current domain version.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Domains

class NSFileProviderDomainVersion

An opaque object that identifies a specific version of a domain.

