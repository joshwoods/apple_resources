

- Network Extension
- NEFilterBrowserFlow
-  response 

Instance Property

# response

An HTTP response of the flow.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var response: URLResponse? { get }
```

## Discussion

This property will be nil until some incoming data is received for this flow.

## See Also

### Getting browser flow properties

var parentURL: URL?

A URL of the web page that’s responsible for the flow’s creation.

var request: URLRequest?

An HTTP request of the flow.

