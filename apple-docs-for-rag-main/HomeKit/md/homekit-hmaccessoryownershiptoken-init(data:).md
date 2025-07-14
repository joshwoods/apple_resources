

- HomeKit
- HMAccessoryOwnershipToken
-  init(data:) 

Initializer

# init(data:)

Creates an ownership token from data.

iOS 13.0+iPadOS 13.0+visionOS 1.0+

``` source
init?(data: Data)
```

## Parameters 

`data`  

Data to be sent to the accessory to prove ownership.

## Discussion

Obtain token data by negotiating with an accessory outside of HomeKit. You typically obtain token data for an accessory that you manufacture.

Token creation can fail if the data doesn’t represent a valid ownership token.

