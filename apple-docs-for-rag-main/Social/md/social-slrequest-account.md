

- Social
- SLRequest
-  account 

Instance Property

# account

Account information used to authenticate the request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
var account: ACAccount! { get set }
```

## Discussion

The account is used to sign a request with OAuth1 services or to add an access token for OAuth2 services. By associating the account with the request, the necessary tokens are added automatically. The default value is `nil`.

