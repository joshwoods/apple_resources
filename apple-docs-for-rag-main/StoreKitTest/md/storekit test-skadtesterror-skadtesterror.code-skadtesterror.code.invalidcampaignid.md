

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.invalidCampaignId 

Case

# SKAdTestError.Code.invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
case invalidCampaignId
```

## Discussion

A campaign ID is an integer that is greater than or equal to one and less than or equal to one hundred.

## See Also

### Older Errors

case signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

case conflictingSource

This error code is unused.

case signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

case conflictingSource

This error code is unused.

