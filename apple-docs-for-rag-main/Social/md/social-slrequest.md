

- Social
-  SLRequest 

Class

# SLRequest

An object that you use to assemble an HTTP request for communicating with a social media service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
class SLRequest
```

## Overview

The SLRequest object encapsulates the properties of an HTTP request, providing a convenient template for you to make requests. You send a request to a social networking service to perform some operation on behalf of the user or to retrieve user information.

HTTP requests have these common components: an HTTP request method (GET, POST, PUT, or DELETE), a URL identifying the operation to perform, a set of query parameters, and an optional multipart POST body that contains additional data. The values for these properties depend on the request you are sending and the target service provider. Refer to each supported social networking site’s documentation for possible values. Links to documentation are provided in Table 1.

Use the init(forServiceType:requestMethod:url:parameters:) method to initialize a newly created `SLRequest` object passing the required property values. Use the addMultipartData(_:withName:type:) to optionally specify a multipart POST body. After you create your request, use the perform(handler:) method to send the request, specifying the handler to call when the request is done.

If you already have a sending mechanism, you can use the preparedURLRequest() method to create the request that you send using an NSURLConnection object. If the request requires user authorization, set the account property to an ACAccount object.

Table 1 Social Services Individual Documentation Sites

| Facebook | https://developers.facebook.com/docs/ |
|----|----|
| Sina Weibo | http://open.weibo.com/wiki/ |
| Twitter | https://dev.twitter.com/docs |
| LinkedIn | https://developer.linkedin.com/rest |

Important

For Sina Weibo integration, users must have the Chinese keyboard enabled. Users can enable this keyboard in Settings \> General \> Keyboard. If a Chinese keyboard is not enabled, users won’t be prompted to sign in to their Sina Weibo account.

## Topics

### Initializing Requests

init!(forServiceType: String!, requestMethod: SLRequestMethod, url: URL!, parameters: [AnyHashable : Any]!)

Initializes a newly created request object with the specified properties.

let SLServiceTypeFacebook: StringDeprecated

let SLServiceTypeTwitter: StringDeprecated

let SLServiceTypeSinaWeibo: StringDeprecated

let SLServiceTypeLinkedIn: StringDeprecated

let SLServiceTypeTencentWeibo: StringDeprecated

### Sending a Request

func perform(handler: SLRequestHandler!)

Performs an asynchronous request and calls the specified handler when done.

typealias SLRequestHandler

The callback handler for a request.

### Providing User Credentials

var account: ACAccount!

Account information used to authenticate the request.

### Getting the Request Details

func preparedURLRequest() -> URLRequest!

Returns an authorized URL request that can be sent using an NSURLConnection object.

var requestMethod: SLRequestMethod

The method to use for this request.

enum SLRequestMethod

Indicates the request method used in the request.

var url: URL!

The destination URL for this request.

var parameters: [AnyHashable : Any]!

The parameters for this request.

### Adding Data to the Request

func addMultipartData(Data!, withName: String!, type: String!, filename: String!)

Specifies a named multipart POST body for this request.

func addMultipartData(Data!, withName: String!, type: String!)

Specifies a named multipart POST body for this request.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

