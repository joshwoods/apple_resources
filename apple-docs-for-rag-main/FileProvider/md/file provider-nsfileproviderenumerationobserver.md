

- File Provider
-  NSFileProviderEnumerationObserver 

Protocol

# NSFileProviderEnumerationObserver

An observer that receives batches of items during enumeration.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
protocol NSFileProviderEnumerationObserver : NSObjectProtocol
```

## Mentioned in 

Defining Your File Provider’s Content

## Topics

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

var suggestedPageSize: Int

The page size that the system recommends.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Content

Defining Your File Provider’s Content

Create enumerators to specify your file provider’s content.

struct NSFileProviderPage

A synchronization point that represents the next batch of items to be returned by an enumerator.

