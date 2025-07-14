

- Foundation
- UserDefaults
-  removePersistentDomain(forName:) 

Instance Method

# removePersistentDomain(forName:)

Removes the contents of the specified persistent domain from the user’s defaults.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removePersistentDomain(forName domainName: String)
```

## Parameters 

`domainName`  

The name of the domain to have its contents removed.

## Discussion

Calling this method is equivalent to initializing a user defaults object with init(suiteName:) passing `domainName`, and calling the removeObject(forKey:) method on each of its keys.

When a persistent domain is changed, an didChangeNotification is posted.

## See Also

### Maintaining Persistent Domains

func persistentDomain(forName: String) -> [String : Any]?

Returns a dictionary representation of the defaults for the specified domain.

func setPersistentDomain([String : Any], forName: String)

Sets a dictionary for the specified persistent domain.

func persistentDomainNames() -> [Any]

Returns an array of the current persistent domain names.

Deprecated

