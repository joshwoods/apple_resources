

- Apple Search Ads
-  NegativeKeyword 

Object

# NegativeKeyword

Negative keyword parameters to use in requests and responses.

Search Ads 2.0+

``` source
object NegativeKeyword
```

## Properties

`adGroupId`

`int64`

The unique identifier of the ad group that the negative keywords belong to. For campaign negative keyword endpoints, the value is `null`.

You can use the EQUALS and IN selector Condition operators with Find Campaign Negative Keywords.

`campaignId`

`int64`

The unique identifier of the campaign that the negative keywords belong to.

You can use the EQUALS and IN selector Condition operators with Find Campaign Negative Keywords.

`deleted`

`boolean`

 (Read-only) 

An indicator of whether the negative keyword is soft-deleted.

`id`

`int64`

 (Read-only) 

A unique identifier for the negative keyword.

You can use the EQUALS and IN selector Condition operators with Find Campaign Negative Keywords.

`matchType`

`string`

 (Required) 

An automated keyword and bidding strategy. Match type can be either `Broad` or `Exact`. See Ad Groups for Search Match use cases.

| **Value** | **Description** |
|----|----|
| `Broad` | Use this value to ensure your ads don’t run on relevant, close variants of a keyword, such as singulars, plurals, misspellings, synonyms, related searches, and phrases that include that term (fully or partially). |
| `Exact` | Use this value for the most control over searches you don’t want your ad to appear in. You can target a specific term and its close variants, such as common misspellings and plurals. |

Possible Values: `EXACT, BROAD`

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

You can use the EQUALS and IN selector Condition operators with Find Campaign Negative Keywords.

`status`

`string`

The user-controlled status to enable or pause the keyword.

Possible Values: `ACTIVE, PAUSED`

`text`

`string`

 (Required) 

The word or phrase to negate in App Store user searches from showing your ad.

## See Also

### Keywords Request and Response Objects

object Keyword

Targeting keyword parameters to use in requests and responses.

object KeywordResponse

A container for the targeting keywords response body.

object KeywordListResponse

The response details of targeting keyword requests.

object KeywordUpdateRequest

Targeting keyword parameters to use in requests and responses.

object NegativeKeywordResponse

A container for the negative keyword response body.

object NegativeKeywordListResponse

The response details of negative keyword requests.

