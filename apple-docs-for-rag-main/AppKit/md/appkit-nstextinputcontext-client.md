

- AppKit
- NSTextInputContext
-  client 

Instance Property

# client

The owner of this input context. (read-only)

macOS 10.6+

``` source
var client: any NSTextInputClient { get }
```

## Discussion

The client (owner) of the input context, typically an `NSView` instance, retains its `NSTextInputContext` instance. The `NSTextInputContext` instance doesn’t retain its client.

## See Also

### Getting the Input Context and Client

class var current: NSTextInputContext?

Returns the current, activated, text input context object.

