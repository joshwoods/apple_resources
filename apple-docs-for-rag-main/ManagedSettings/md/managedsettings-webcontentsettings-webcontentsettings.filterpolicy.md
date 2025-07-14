

- ManagedSettings
- WebContentSettings
-  WebContentSettings.FilterPolicy 

Enumeration

# WebContentSettings.FilterPolicy

The policies available for filtering web content based on specific web domains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
enum FilterPolicy
```

## Topics

### Providing Filters and Exceptions

case all(except: Set&lt;WebDomain>)

The system blocks all websites except the ones you specify.

case auto(Set&lt;WebDomain>, except: Set&lt;WebDomain>)

The system blocks adult content.

case none

The policy doesn’t affect any domains.

case specific(Set&lt;WebDomain>)

The policy blocks the specified domains.

### Comparing Policies

static func == (WebContentSettings.FilterPolicy, WebContentSettings.FilterPolicy) -> Bool

Returns a Boolean value that indicates whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Filtering Web Domains

var blockedByFilter: WebContentSettings.FilterPolicy?

The current policy for filtering websites.

static let blockedByFilter: SettingMetadata&lt;WebContentSettings.FilterPolicy>

A description of the setting that controls which websites a user can access.

