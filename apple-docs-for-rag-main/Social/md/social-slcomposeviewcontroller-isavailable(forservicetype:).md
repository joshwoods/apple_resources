

- Social
- SLComposeViewController
-  isAvailable(forServiceType:) 

Type Method

# isAvailable(forServiceType:)

Returns A Boolean value that indicates whether you can send a request for a particular service type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
class func isAvailable(forServiceType serviceType: String!) -> Bool
```

## Parameters 

`serviceType`  

The social networking service. For a list of possible values, see Service Type Constants.

## Return Value

Returns a Boolean value that indicates whether the service is accessible and whether at least one account is set up.

## Discussion

For the account to be available, the user must be logged into the social service in the device settings.

## See Also

### Checking the Social Service Type

var serviceType: String!

Specifies the social-networking service.

