

- AppKit
- NSScrubber
-  dataSource 

Instance Property

# dataSource

The object that provides the data for the scrubber.

macOS 10.12.2+

``` source
@MainActor
weak var dataSource: (any NSScrubberDataSource)? { get set }
```

## See Also

### Configuring the scrubber

var delegate: (any NSScrubberDelegate)?

The object that acts as the delegate of the scrubber.

