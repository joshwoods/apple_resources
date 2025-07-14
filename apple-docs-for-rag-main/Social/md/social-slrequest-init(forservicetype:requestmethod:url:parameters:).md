

- Social
- SLRequest
-  init(forServiceType:requestMethod:url:parameters:) 

Initializer

# init(forServiceType:requestMethod:url:parameters:)

Initializes a newly created request object with the specified properties.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
init!(
    forServiceType serviceType: String!,
    requestMethod: SLRequestMethod,
    url: URL!,
    parameters: [AnyHashable : Any]!
)
```

## Parameters 

`serviceType`  

The social networking service type. For possible values, see `Service Type Constants`.

`requestMethod`  

The method to use for this HTTP request. For possible values, see SLRequestMethod.

`url`  

The destination URL for this HTTP request. The values and formatting for the URL are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

`parameters`  

The parameters for this HTTP request. The values and formatting are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## Return Value

The newly initialized request object.

## Discussion

Use this method to initialize an `SLRequest`. The value and formatting of each parameter is dependent on the target service.

## See Also

### Initializing Requests

let SLServiceTypeFacebook: StringDeprecated

let SLServiceTypeTwitter: StringDeprecated

let SLServiceTypeSinaWeibo: StringDeprecated

let SLServiceTypeLinkedIn: StringDeprecated

let SLServiceTypeTencentWeibo: StringDeprecated

