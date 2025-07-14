

- ManagedSettings
- WebContentSettings
- WebContentSettings.FilterPolicy
-  WebContentSettings.FilterPolicy.none 

Case

# WebContentSettings.FilterPolicy.none

The policy doesn’t affect any domains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case none
```

## See Also

### Providing Filters and Exceptions

case all(except: Set&lt;WebDomain>)

The system blocks all websites except the ones you specify.

case auto(Set&lt;WebDomain>, except: Set&lt;WebDomain>)

The system blocks adult content.

case specific(Set&lt;WebDomain>)

The policy blocks the specified domains.

