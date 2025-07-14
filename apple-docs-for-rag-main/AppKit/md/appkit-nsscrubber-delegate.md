

- AppKit
- NSScrubber
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the scrubber.

macOS 10.12.2+

``` source
@MainActor
weak var delegate: (any NSScrubberDelegate)? { get set }
```

## See Also

### Configuring the scrubber

var dataSource: (any NSScrubberDataSource)?

The object that provides the data for the scrubber.

