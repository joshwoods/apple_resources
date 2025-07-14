

- ManagedSettings
- WebContentSettings
- WebContentSettings.FilterPolicy
-  WebContentSettings.FilterPolicy.auto(\_:except:) 

Case

# WebContentSettings.FilterPolicy.auto(\_:except:)

The system blocks adult content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case auto(
    Set = [],
    except: Set = []
)
```

## Discussion

The system also blocks websites you provide in `domains`. The system allows websites you provide in `except`, overriding the adult content filter and `domains` set. Your app can block up to 50 web domains and specify up to 50 web domains exceptions at once.

## See Also

### Providing Filters and Exceptions

case all(except: Set&lt;WebDomain>)

The system blocks all websites except the ones you specify.

case none

The policy doesn’t affect any domains.

case specific(Set&lt;WebDomain>)

The policy blocks the specified domains.

