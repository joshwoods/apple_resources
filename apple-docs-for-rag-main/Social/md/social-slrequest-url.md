

- Social
- SLRequest
-  url 

Instance Property

# url

The destination URL for this request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
var url: URL! { get }
```

## Discussion

Use this property to look up the URL of the HTTP request that was set in init(forServiceType:requestMethod:url:parameters:). Possible values are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Getting the Request Details

func preparedURLRequest() -> URLRequest!

Returns an authorized URL request that can be sent using an NSURLConnection object.

var requestMethod: SLRequestMethod

The method to use for this request.

enum SLRequestMethod

Indicates the request method used in the request.

var parameters: [AnyHashable : Any]!

The parameters for this request.

