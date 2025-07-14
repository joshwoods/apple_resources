

- Apple Search Ads
-  Ads 

API Collection

# Ads

Assign an ad creative to an ad group.

## Overview

You use an Ad object to assign an ad creative to an ad group. You can assign one active ad per ad group. See also Ad Rejection Reasons.

## Topics

### Ad Endpoints

Create an Ad

Creates an ad in an ad group with a creative.

Find Ads

Finds ads within a campaign by selector criteria.

Find Ads (org-level)

Fetches ads within an organization by selector criteria.

Get an Ad

Fetches an ad assigned to an ad group by identifier.

Get All Ads

Fetches all ads assigned to an ad group.

Update an Ad

Updates an ad in an ad group.

Delete an Ad

Deletes an ad from an ad group.

### Ad Request and Response Objects

object Ad

The assignment of a creative to an ad group.

object AdCreate

The request to create an ad, and assign a creative to an ad group.

object AdUpdate

The request to update an ad.

object AdResponse

The response to an ad request.

object AdListResponse

The response to a request that returns a list of ads.

### Data Types

type AdServingStateReasons

Reasons the system provides when an ad isn’t running.

type AdStatus

The user-controlled status of the ad.

type AdServingStatus

The status of whether the ad is serving.

## See Also

### Custom Product Page Ads

Ad Rejection Reasons

Review reasons for an ad rejection.

Creatives

Create and manage ad creatives within your organization.

Custom Product Pages

View Custom Product Page details.

