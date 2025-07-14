

- Social
- SLComposeViewController
-  serviceType 

Instance Property

# serviceType

Specifies the social-networking service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
var serviceType: String! { get }
```

## Discussion

The value of this property is set when you initialize a social compose view controller in init(forServiceType:). Each social view controller you present is connected to only one social service at a time. Use this property to check which service your social view controller has specified. For a list of possible values, see Service Type Constants.

## See Also

### Checking the Social Service Type

class func isAvailable(forServiceType: String!) -> Bool

Returns A Boolean value that indicates whether you can send a request for a particular service type.

