

- Core Telephony
- CTSubscriber
-  identifier 

Instance Property

# identifier

An implementation-defined identifier used to correlate this subscriber with information vended by other APIs.

iOS 12.1+iPadOS 12.1+

``` source
var identifier: String { get }
```

## Discussion

The format of the identifier can change across software releases. Therefore, do not persist this identifier.

