

- StoreKit Test
- SKAdTestError
-  invalidCampaignId 

Type Property

# invalidCampaignId

The campaign ID isn’t an integer between one and one hundred.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
static var invalidCampaignId: SKAdTestError.Code { get }
```

## Discussion

A campaign ID is an integer that is greater than or equal to one and less than or equal to one hundred.

## See Also

### Getting Older Errors

static var signatureMissingCampaignId: SKAdTestError.Code

The signature is missing the campaign identifier, in the testing environment.

static var conflictingSource: SKAdTestError.Code

This error code is unused.

