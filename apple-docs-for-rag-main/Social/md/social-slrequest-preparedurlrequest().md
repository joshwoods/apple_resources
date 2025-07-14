

- Social
- SLRequest
-  preparedURLRequest() 

Instance Method

# preparedURLRequest()

Returns an authorized URL request that can be sent using an NSURLConnection object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
func preparedURLRequest() -> URLRequest!
```

## Return Value

An OAuth-compatible `NSURLRequest` object that allows an app to act on behalf of the user, while keeping the user’s password private. The `NSURLRequest` is signed as OAuth1 by default, or OAuth2 by adding the appropriate token based on the user’s account.

## Discussion

Use this method to modify your request before sending. By setting the account correctly, this method will automatically add any necessary tokens.

## See Also

### Getting the Request Details

var requestMethod: SLRequestMethod

The method to use for this request.

enum SLRequestMethod

Indicates the request method used in the request.

var url: URL!

The destination URL for this request.

var parameters: [AnyHashable : Any]!

The parameters for this request.

