

- ManagedSettings
- WebContentSettings
- WebContentSettings.FilterPolicy
-  WebContentSettings.FilterPolicy.specific(\_:) 

Case

# WebContentSettings.FilterPolicy.specific(\_:)

The policy blocks the specified domains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case specific(Set)
```

## Discussion

Your app can block up to 50 web domains at once.

## See Also

### Providing Filters and Exceptions

case all(except: Set&lt;WebDomain>)

The system blocks all websites except the ones you specify.

case auto(Set&lt;WebDomain>, except: Set&lt;WebDomain>)

The system blocks adult content.

case none

The policy doesn’t affect any domains.

