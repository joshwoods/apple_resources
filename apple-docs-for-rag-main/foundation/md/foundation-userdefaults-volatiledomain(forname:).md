

- Foundation
- UserDefaults
-  volatileDomain(forName:) 

Instance Method

# volatileDomain(forName:)

Returns the dictionary for the specified volatile domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func volatileDomain(forName domainName: String) -> [String : Any]
```

## Parameters 

`domainName`  

The domain whose keys and values you want.

## Return Value

The dictionary of keys and values belonging to the domain. The keys in the dictionary are names of defaults, and the value corresponding to each key is a property list object (`NSData`, `NSString`, `NSNumber`, `NSDate`, `NSArray`, or `NSDictionary`).

## See Also

### Maintaining Volatile Domains

var volatileDomainNames: [String]

The current volatile domain names.

func setVolatileDomain([String : Any], forName: String)

Sets the dictionary for the specified volatile domain.

func removeVolatileDomain(forName: String)

Removes the specified volatile domain from the user’s defaults.

