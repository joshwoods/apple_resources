

- Metal
- MTLEvent
-  label 

Instance Property

# label

A string that identifies the event.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Event

var device: (any MTLDevice)?

The device object that created the event.

**Required**

