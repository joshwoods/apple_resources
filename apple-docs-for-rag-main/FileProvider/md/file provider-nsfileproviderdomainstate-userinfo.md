

- File Provider
- NSFileProviderDomainState
-  userInfo 

Instance Property

# userInfo

Global state information about the current domain version.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
var userInfo: [AnyHashable : Any] { get }
```

**Required**

## Discussion

Use this dictionary to add state information to the domain. You can then access the userInfo dictionary in predicates for user interactions, file provider actions, and File Provider UI actions using the `domainUserInfo` context key.

This dictionary must only contain the following types for both its keys and values:

- NSString

- NSNumber

- NSDate

- NSPersonNameComponents

The system expects you to update the `domainVersion` whenever the value of the userInfo dictionary changes.

## See Also

### Accessing State Data

var domainVersion: NSFileProviderDomainVersion

An opaque object that uniquely identifies the domain’s version.

**Required**

