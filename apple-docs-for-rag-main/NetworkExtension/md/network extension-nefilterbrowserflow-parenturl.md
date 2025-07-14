

- Network Extension
- NEFilterBrowserFlow
-  parentURL 

Instance Property

# parentURL

A URL of the web page that’s responsible for the flow’s creation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var parentURL: URL? { get }
```

## Discussion

This property will be non-nil only if the flow is loading a resource into a frame. In that case, this property will be set to the URL of the web page containing the frame.

## See Also

### Getting browser flow properties

var request: URLRequest?

An HTTP request of the flow.

var response: URLResponse?

An HTTP response of the flow.

