

- Foundation
- NSProtocolChecker
-  init(target:protocol:) 

Initializer

# init(target:protocol:)

Initializes a newly allocated `NSProtocolChecker` instance that will forward any messages in `aProtocol` to `anObject`, the protocol checker’s target.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    target anObject: NSObject,
    protocol aProtocol: Protocol
)
```

## Discussion

Thus, the checker can be vended in lieu of `anObject` to restrict the messages that can be sent to `anObject`. If `anObject` is allowed to be freed or dereferenced by clients, the `free` method should be included in `aProtocol`.

