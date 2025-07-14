

- Foundation
- URLSessionTaskTransactionMetrics
-  response 

Instance Property

# response

The transaction response.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var response: URLResponse? { get }
```

## Discussion

This property is `nil` if an error occurred and no response was generated.

## See Also

### Accessing request and response

var request: URLRequest

The transaction request.

