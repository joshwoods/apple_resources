

- File Provider
- NSFileProviderEnumerationObserver
-  finishEnumerating(upTo:) 

Instance Method

# finishEnumerating(upTo:)

Tells the observer that all of the items have been enumerated up to the specified page.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
func finishEnumerating(upTo nextPage: NSFileProviderPage?)
```

**Required**

## Mentioned in 

Defining Your File Provider’s Content

## See Also

### Observing Item Enumeration

func didEnumerate([any NSFileProviderItemProtocol])

Provides a batch of enumerated items.

**Required**

func finishEnumeratingWithError(any Error)

Tells the observer that an error occurred during item enumeration.

**Required**

var suggestedPageSize: Int

The page size that the system recommends.

