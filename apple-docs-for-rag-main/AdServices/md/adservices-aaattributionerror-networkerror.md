

- AdServices
- AAAttributionError
-  networkError 

Type Property

# networkError

The server is unable to provide a token because the internet isn’t available.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 11.1+visionOS 1.0+

``` source
static var networkError: AAAttributionError.Code { get }
```

## Discussion

To receive an attribution token, you must have unimpeded internet access. Make sure you’re not using a simulator when generating a token.

## See Also

### Error codes

static var internalError: AAAttributionError.Code

The server is unable to provide a token because of an internal error.

static var platformNotSupported: AAAttributionError.Code

The server is unable to provide a token because of an unsupported operating system.

enum Code

The error code that the parent class issues.

