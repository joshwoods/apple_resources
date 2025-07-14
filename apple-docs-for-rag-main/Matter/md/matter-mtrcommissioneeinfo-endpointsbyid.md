

- Matter
- MTRCommissioneeInfo
-  endpointsById 

Instance Property

# endpointsById

Endpoint information for all endpoints of the commissionee. Will be present only if readEndpointInformation is set to YES on MTRCommissioningParameters.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
var endpointsById: [NSNumber : MTREndpointInfo]? { get }
```

## Discussion

Use `rootEndpoint` and `-[MTREndpointInfo children]` to traverse endpoints in composition order.

