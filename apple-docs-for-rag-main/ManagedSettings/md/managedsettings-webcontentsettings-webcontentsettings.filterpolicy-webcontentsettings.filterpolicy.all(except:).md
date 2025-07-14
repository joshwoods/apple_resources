

- ManagedSettings
- WebContentSettings
- WebContentSettings.FilterPolicy
-  WebContentSettings.FilterPolicy.all(except:) 

Case

# WebContentSettings.FilterPolicy.all(except:)

The system blocks all websites except the ones you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case all(except: Set = [])
```

## Discussion

Your app can specify up to 50 web domains exceptions.

## See Also

### Providing Filters and Exceptions

case auto(Set&lt;WebDomain>, except: Set&lt;WebDomain>)

The system blocks adult content.

case none

The policy doesn’t affect any domains.

case specific(Set&lt;WebDomain>)

The policy blocks the specified domains.

