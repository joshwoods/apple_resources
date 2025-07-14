

- SwiftUI
- SubscriptionView
-  publisher 

Instance Property

# publisher

The `Publisher` that is being subscribed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var publisher: PublisherType
```

## See Also

### Managing the subscription

var action: (PublisherType.Output) -> Void

The `Action` executed when `publisher` emits an event.

var content: Content

The content view.

