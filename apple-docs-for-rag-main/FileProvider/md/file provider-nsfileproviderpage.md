

- File Provider
-  NSFileProviderPage 

Structure

# NSFileProviderPage

A synchronization point that represents the next batch of items to be returned by an enumerator.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
struct NSFileProviderPage
```

## Discussion

Your file provider should populate the page with the information it needs to partition items into batches and to systematically return a batch of data at a time. For example, a simple page could contain the index of the next item to return. A request to enumerate items from that page would then return a batch of items starting at the specified index.

## Topics

### Page Constants

static let initialPageSortedByName: NSData

The initial batch of items when sorted by name.

static let initialPageSortedByDate: NSData

The initial batch of items when sorted by date.

### Initializers

init(Data)

Creates a new page structure from the given raw value.

init(rawValue: Data)

Creates a new page structure from the given raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Content

Defining Your File Provider’s Content

Create enumerators to specify your file provider’s content.

protocol NSFileProviderEnumerationObserver

An observer that receives batches of items during enumeration.

