

- Vision
- VNRequestProgressProviding
-  indeterminate 

Instance Property

# indeterminate

A Boolean set to true when a request can’t determine its progress in fractions completed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var indeterminate: Bool { get }
```

**Required**

## Discussion

A value of true doesn’t mean that the request will run forever. Rather, it means that the nature of the request can’t be broken down into identifiable fractions to report. The progressHandler will still be called at suitable intervals.

## See Also

### Tracking Progress

var progressHandler: VNRequestProgressHandler

A block of code executed periodically during a Vision request to report progress on long-running tasks.

**Required**

