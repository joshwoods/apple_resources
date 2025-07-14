

- App Store Server API
-  extendReasonCode 

Type

# extendReasonCode

The code that represents the reason for the subscription-renewal-date extension.

App Store Server API 1.1+

``` source
int32 extendReasonCode
```

## Possible Values 

`0`  

Undeclared; no information provided.

`1`  

The renewal-date extension is for customer satisfaction.

`2`  

The renewal-date extension is for other reasons.

`3`  

The renewal-date extension is due to a service issue or outage.

## Discussion

For more information about requesting subscription-renewal-date extensions, see Extending the renewal date for auto-renewable subscriptions.

## See Also

### Request data types

type extendByDays

The number of days to extend the subscription renewal date.

type requestIdentifier

A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.

