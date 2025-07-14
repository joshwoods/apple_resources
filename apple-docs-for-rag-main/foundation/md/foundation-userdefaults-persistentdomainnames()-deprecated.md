

- Foundation
- UserDefaults
-  persistentDomainNames() Deprecated

Instance Method

# persistentDomainNames()

Returns an array of the current persistent domain names.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func persistentDomainNames() -> [Any]
```

Deprecated

Instead of using this method, you should track the domains you add if you want to later retrieve them with persistentDomain(forName:).

## Return Value

An array of `NSString` objects containing the domain names.

## Discussion

You can get the keys and values for each domain by passing the returned domain names to the persistentDomain(forName:) method.

## See Also

### Maintaining Persistent Domains

func persistentDomain(forName: String) -> [String : Any]?

Returns a dictionary representation of the defaults for the specified domain.

func setPersistentDomain([String : Any], forName: String)

Sets a dictionary for the specified persistent domain.

func removePersistentDomain(forName: String)

Removes the contents of the specified persistent domain from the user’s defaults.

