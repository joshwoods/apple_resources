

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.signatureMissingCampaignId 

Case

# SKAdTestError.Code.signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
case signatureMissingCampaignId
```

## Discussion

Be sure to include the campaign identifier when you create and validate an ad impression in the testing environment.

## See Also

### Older Errors

case invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

case conflictingSource

This error code is unused.

case invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

case conflictingSource

This error code is unused.

