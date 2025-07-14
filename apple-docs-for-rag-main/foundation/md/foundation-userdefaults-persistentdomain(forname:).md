

- Foundation
- UserDefaults
-  persistentDomain(forName:) 

Instance Method

# persistentDomain(forName:)

Returns a dictionary representation of the defaults for the specified domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func persistentDomain(forName domainName: String) -> [String : Any]?
```

## Parameters 

`domainName`  

The name of the domain to be represented.

## Return Value

A dictionary containing keys for each default name and their corresponding default values.

## Discussion

Calling this method is equivalent to initializing a user defaults object with init(suiteName:) passing `domainName` and calling the dictionaryRepresentation() method on it.

## See Also

### Maintaining Persistent Domains

func setPersistentDomain([String : Any], forName: String)

Sets a dictionary for the specified persistent domain.

func removePersistentDomain(forName: String)

Removes the contents of the specified persistent domain from the user’s defaults.

func persistentDomainNames() -> [Any]

Returns an array of the current persistent domain names.

Deprecated

