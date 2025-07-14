

- Apple Search Ads
-  CampaignUpdate 

Object

# CampaignUpdate

The list of campaign fields that are updatable.

Search Ads 2.0+

``` source
object CampaignUpdate
```

## Properties

`budgetAmount`

Money

The lifetime budget amount available to a campaign.

- Campaigns require a `dailyBudgetAmount` or a `budgetAmount`, or both.

- If you update a `budgetAmount`, the updated amount must be greater than the previous `budgetAmount` and must exceed the lifetime spend of the campaign.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

This field is updatable.

`budgetOrders`

`[int64]`

The budget orders that you assign to the campaign. This applies only to campaigns with a line-of-credit payment model. See Budget Orders.

`countriesOrRegions`

`[string]`

The App Store geoterritories where you’re promoting your app. The default value is `US`.

This field requires an ISO country code value for the locations where you’re promoting.

`dailyBudgetAmount`

Money

Your daily budget.

- Campaigns require a `dailyBudgetAmount` or a `budgetAmount`, or both.

- Your `dailyBudgetAmount` must be less than your `budgetAmount`.

- Your `dailyBudgetAmount` must be greater than or equal to the `defaultBidAmount` in your AdGroup.

You can use the `EQUALS`, `LESS_THAN`, and `GREATER_THAN` selector Condition operators with Find Campaigns.

This field is updatable.

`locInvoiceDetails`

LOCInvoiceDetails

The standard invoice details you can set and edit using the LOCInvoiceDetails object.

`name`

`string`

The name of the campaign, which is unique within an organization.

`status`

`string`

The user-controlled status to enable or pause the campaign.

Possible Values: `ENABLED, PAUSED`

## See Also

### Campaign Request and Response Objects

object Campaign

The response to a request to create and fetch campaigns.

object CampaignResponse

A container for the campaign response body.

object Campaign.CountryOrRegionServingStateReasons

Reasons why a campaign can’t run.

object CampaignListResponse

The response details of campaign requests.

object UpdateCampaignRequest

The payload properties to clear geotargeting from a campaign.

