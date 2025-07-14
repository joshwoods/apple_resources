

- Foundation
- UserDefaults
-  setVolatileDomain(\_:forName:) 

Instance Method

# setVolatileDomain(\_:forName:)

Sets the dictionary for the specified volatile domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setVolatileDomain(
    _ domain: [String : Any],
    forName domainName: String
)
```

## Parameters 

`domain`  

The dictionary of keys and values you want to assign to the domain.

`domainName`  

The domain whose keys and values you want to set.

## Discussion

This method raises an `NSInvalidArgumentException` if a volatile domain with the specified name already exists.

## See Also

### Maintaining Volatile Domains

var volatileDomainNames: [String]

The current volatile domain names.

func volatileDomain(forName: String) -> [String : Any]

Returns the dictionary for the specified volatile domain.

func removeVolatileDomain(forName: String)

Removes the specified volatile domain from the user’s defaults.

