

- File Provider
- NSFileProviderPendingSetEnumerator
-  domainVersion 

Instance Property

# domainVersion

The domain version when the system last refreshed the pending set.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var domainVersion: NSFileProviderDomainVersion? { get }
```

**Required**

## Discussion

The system sets this property when you call the enumerator’s methods. The value is initially `nil`.

## See Also

### Accessing Refresh Data

var refreshInterval: TimeInterval

The amount of time, in seconds, between updates to the pending set.

**Required**

