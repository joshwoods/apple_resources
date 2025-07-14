

- System Extensions
- OSSystemExtensionRequest
-  delegate 

Instance Property

# delegate

A delegate to receive updates about the progress of a request.

macOS 10.15+

``` source
weak var delegate: (any OSSystemExtensionRequestDelegate)? { get set }
```

## See Also

### Working with a Delegate

protocol OSSystemExtensionRequestDelegate

A type that receives updates about the progress of a request.

