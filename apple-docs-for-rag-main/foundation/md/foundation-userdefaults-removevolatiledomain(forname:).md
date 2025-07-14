

- Foundation
- UserDefaults
-  removeVolatileDomain(forName:) 

Instance Method

# removeVolatileDomain(forName:)

Removes the specified volatile domain from the user’s defaults.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeVolatileDomain(forName domainName: String)
```

## Parameters 

`domainName`  

The volatile domain you want to remove.

## See Also

### Maintaining Volatile Domains

var volatileDomainNames: [String]

The current volatile domain names.

func volatileDomain(forName: String) -> [String : Any]

Returns the dictionary for the specified volatile domain.

func setVolatileDomain([String : Any], forName: String)

Sets the dictionary for the specified volatile domain.

