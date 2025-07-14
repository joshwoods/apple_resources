

- Social
-  SLRequestHandler 

Type Alias

# SLRequestHandler

The callback handler for a request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+

``` source
typealias SLRequestHandler = (Data?, HTTPURLResponse?, (any Error)?) -> Void
```

## Discussion

The parameters for this handler are:

`responseData`  
The data returned by the request. The format of this data is dependent on the target service.

`urlResponse`  
The URL response returned by the request that includes the HTTP response codes.

`error`  
An error identifier.

Possible values are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Sending a Request

func perform(handler: SLRequestHandler!)

Performs an asynchronous request and calls the specified handler when done.

