

- Apple Search Ads
-  KeywordUpdateRequest 

Object

# KeywordUpdateRequest

Targeting keyword parameters to use in requests and responses.

Search Ads 2.0.9+

``` source
object KeywordUpdateRequest
```

## Properties

`adGroupId`

`int64`

The unique identifier for the ad group that the targeting keyword belongs to.

`bidAmount`

Money

The maximum cost-per-tap/impression bid amount. This is the offer price for a keyword in a bidding auction.

If you set `automatedKeywordsOptIn=true` in Update an Ad Group, the bid uses optimized keywords with the `defaultBidAmount`.

`deleted`

`boolean`

 (Read-only) 

An indicator of whether the keyword is soft-deleted.

Default: `false`

`id`

`int64`

 (Read-only) 

A unique identifier for the targeting keyword in the payload to update keyword bids or statuses. This `keywordId` is specific to a particular ad group and match type that you use to update bid amounts.

`matchType`

`string`

 (Required) 

An automated keyword and bidding strategy. Match type can be either `Broad` or `Exact`. See Ad Groups for Search Match use cases.

| **Value** | **Description** |
|----|----|
| `Broad` | Use this value to ensure your ads don’t run on relevant, close variants of a keyword, such as singulars, plurals, misspellings, synonyms, related searches, and phrases that include that term (fully or partially). |
| `Exact` | Use this value for the most control over searches your ad may appear in. You can target a specific term and its close variants, such as common misspellings and plurals. Your ad may receive fewer impressions as a result, but your tap-through rates (TTRs) and conversions on those impressions may be higher because you’re reaching users most interested in your app. |

Default: `BROAD`

Possible Values: `BROAD, EXACT`

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

`status`

`string`

The user-controlled status to enable or pause the keyword.

Possible Values: `ACTIVE, PAUSED`

`text`

`string`

 (Required) 

The word or phrase to match in App Store user searches to show your ad.

## See Also

### Keywords Request and Response Objects

object Keyword

Targeting keyword parameters to use in requests and responses.

object NegativeKeyword

Negative keyword parameters to use in requests and responses.

object KeywordResponse

A container for the targeting keywords response body.

object KeywordListResponse

The response details of targeting keyword requests.

object NegativeKeywordResponse

A container for the negative keyword response body.

object NegativeKeywordListResponse

The response details of negative keyword requests.

