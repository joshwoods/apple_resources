

- Apple Search Ads
-  Ad Rejection Reasons 

API Collection

# Ad Rejection Reasons

Review reasons for an ad rejection.

## Overview

Ads require approval by Apple. While in review, your Ad is on hold. After approval, the AdServingStatus changes to `RUNNING` unless you schedule it to start on a specific date or Update an Ad status to `PAUSED` while in review.

Note

In 4.9 release, all previously rejected Today tab ad creatives were `PAUSED` and resubmitted for re-review. You need to update the status to `ENABLED` after the re-review. See Update an Ad.

Use Find Ad Creative Rejection Reasons or Get Ad Creative Rejection Reasons to look up rejection reasons. See ProductPageReason for rejection reason descriptions.

## Topics

### Ad Rejections

Find Ad Creative Rejection Reasons

Fetches ad creative rejection reasons.

Get Ad Creative Rejection Reasons

Fetches ad creative rejection reasons by custom product page ID.

Find App Assets

Fetches app asset metadata by adam ID.

### Ad Rejection Reason Objects

object AppAsset

The app assets associated with an adam ID.

object AppAssetListResponse

The response to a request that returns a list of app assets.

object ProductPageReason

The ad creative rejection reason based on a product page.

object ProductPageReasonListResponse

The response to a request that returns a list of product page rejection reasons.

object ProductPageReasonResponse

A container for product page reasons.

### Data Types

type ReasonLevel

The level at which the system applies an ad rejection reason.

## See Also

### Custom Product Page Ads

Ads

Assign an ad creative to an ad group.

Creatives

Create and manage ad creatives within your organization.

Custom Product Pages

View Custom Product Page details.

