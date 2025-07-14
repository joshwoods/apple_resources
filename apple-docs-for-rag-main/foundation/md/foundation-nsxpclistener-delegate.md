

- Foundation
- NSXPCListener
-  delegate 

Instance Property

# delegate

The delegate for the listener.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any NSXPCListenerDelegate)? { get set }
```

## Discussion

If no delegate is set, all new connections are rejected. See the documentation for NSXPCListenerDelegate for implementation details.

