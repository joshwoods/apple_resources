

- Foundation
- UserDefaults
-  setPersistentDomain(\_:forName:) 

Instance Method

# setPersistentDomain(\_:forName:)

Sets a dictionary for the specified persistent domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setPersistentDomain(
    _ domain: [String : Any],
    forName domainName: String
)
```

## Parameters 

`domain`  

A dictionary of keys and values you want to assign to the domain.

`domainName`  

The name of the domain whose contents you want to set.

## Discussion

Calling this method is equivalent to initializing a user defaults object with init(suiteName:) passing `domainName`, and calling the set(_:forKey:) method for each key-value pair in `domain`.

When a persistent domain is changed, an didChangeNotification is posted.

## See Also

### Maintaining Persistent Domains

func persistentDomain(forName: String) -> [String : Any]?

Returns a dictionary representation of the defaults for the specified domain.

func removePersistentDomain(forName: String)

Removes the contents of the specified persistent domain from the user’s defaults.

func persistentDomainNames() -> [Any]

Returns an array of the current persistent domain names.

Deprecated

