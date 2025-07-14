

- AppKit
-  NSScrubberDataSource 

Protocol

# NSScrubberDataSource

A set of methods that a scrubber data source object implements to provide items to the scrubber from an associated data collection in your app.

macOS

``` source
protocol NSScrubberDataSource : NSObjectProtocol
```

## Topics

### Getting the scrubber metrics

func numberOfItems(for: NSScrubber) -> Int

Asks the data source for the number of items in the scrubber.

**Required**

### Getting views for items

func scrubber(NSScrubber, viewForItemAt: Int) -> NSScrubberItemView

Asks the data source object for the view the corresponds to the specified item in the scrubber.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Scrubbers

class NSScrubber

A customizable item picker control for the Touch Bar.

protocol NSScrubberDelegate

A set of methods that a scrubber delegate implements to respond to user interactions.

