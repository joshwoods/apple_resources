

- Social
- SLRequest
-  requestMethod 

Instance Property

# requestMethod

The method to use for this request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
var requestMethod: SLRequestMethod { get }
```

## Discussion

Use this property to look up the method of the HTTP request that was set in init(forServiceType:requestMethod:url:parameters:). Possible values are described in SLRequestMethod.

## See Also

### Getting the Request Details

func preparedURLRequest() -> URLRequest!

Returns an authorized URL request that can be sent using an NSURLConnection object.

enum SLRequestMethod

Indicates the request method used in the request.

var url: URL!

The destination URL for this request.

var parameters: [AnyHashable : Any]!

The parameters for this request.

