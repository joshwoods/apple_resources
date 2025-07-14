

- CryptoTokenKit
- TKTokenDriver
-  delegate 

Instance Property

# delegate

The token driver delegate.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
weak var delegate: (any TKTokenDriverDelegate)? { get set }
```

## See Also

### Responding to Token Creation

protocol TKTokenDriverDelegate

The interface that a token driver delegate implements to respond to token creation events.

typealias ClassID

The type of the class identifier for the token driver.

class Configuration

A configuration for one class of token.

