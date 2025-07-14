

- File Provider
- NSFileProviderEnumerationObserver
-  suggestedPageSize 

Instance Property

# suggestedPageSize

The page size that the system recommends.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional var suggestedPageSize: Int { get }
```

## Discussion

The system suggests a page size to optimize performance based on the enumeration’s context. The system can request the enumeration of a container for various reasons, such as if the user opens the directory in Finder, opens a file in an application, or if the system needs to materialize the contents of a directory. Each case has its own performance profile.

While using the suggested page size helps ensure the best user experience, the system enforces a maximum of 100 times the suggested size.

## See Also

### Observing Item Enumeration

func didEnumerate([any NSFileProviderItemProtocol])

Provides a batch of enumerated items.

**Required**

func finishEnumerating(upTo: NSFileProviderPage?)

Tells the observer that all of the items have been enumerated up to the specified page.

**Required**

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during item enumeration.

**Required**

