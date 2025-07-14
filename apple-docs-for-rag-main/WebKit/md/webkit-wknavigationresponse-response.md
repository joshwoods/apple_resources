

- WebKit
- WKNavigationResponse
-  response 

Instance Property

# response

The frame’s response.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@NSCopying @MainActor
var response: URLResponse { get }
```

## Discussion

Allowing a navigation response with a MIME type that WebKit can’t display causes the navigation to fail.

