

- Network
- NWConnection
-  receiveDiscontiguous(minimumIncompleteLength:maximumLength:completion:) 

Instance Method

# receiveDiscontiguous(minimumIncompleteLength:maximumLength:completion:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@preconcurrency
final func receiveDiscontiguous(
    minimumIncompleteLength: Int,
    maximumLength: Int,
    completion: @escaping (DispatchData?, NWConnection.ContentContext?, Bool, NWError?) -> Void
)
```

