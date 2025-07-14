

- StoreKit Test
- SKAdTestError
-  signatureMissingCampaignId 

Type Property

# signatureMissingCampaignId

The signature is missing the campaign identifier, in the testing environment.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+

``` source
static var signatureMissingCampaignId: SKAdTestError.Code { get }
```

## Discussion

Be sure to include the campaign identifier when you create and validate an ad impression in the testing environment.

## See Also

### Getting Older Errors

static var invalidCampaignId: SKAdTestError.Code

The campaign ID isn’t an integer between one and one hundred.

static var conflictingSource: SKAdTestError.Code

This error code is unused.

