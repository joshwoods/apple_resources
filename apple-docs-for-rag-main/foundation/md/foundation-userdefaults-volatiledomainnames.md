

- Foundation
- UserDefaults
-  volatileDomainNames 

Instance Property

# volatileDomainNames

The current volatile domain names.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var volatileDomainNames: [String] { get }
```

## Discussion

The domain names are represented as strings. You can get the contents of each domain by passing the returned domain names to the volatileDomain(forName:) method.

## See Also

### Maintaining Volatile Domains

func volatileDomain(forName: String) -> [String : Any]

Returns the dictionary for the specified volatile domain.

func setVolatileDomain([String : Any], forName: String)

Sets the dictionary for the specified volatile domain.

func removeVolatileDomain(forName: String)

Removes the specified volatile domain from the user’s defaults.

