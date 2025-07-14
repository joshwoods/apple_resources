

- Network
- NWPathMonitor
-  currentPath 

Instance Property

# currentPath

The currently available network path observed by the path monitor.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final var currentPath: NWPath { get set }
```

## See Also

### Handling Path Updates

var pathUpdateHandler: ((NWPath) -> Void)?

A handler that receives network path updates.

