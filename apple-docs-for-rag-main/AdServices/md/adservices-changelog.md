

- AdServices
-  Changelog 

Article

# Changelog

A log of Ad Services framework updates.

## Overview

| Release date | Release details |
|----|----|
| March, 2025 | View-through attribution is introduced on March 27, 2025. A new attribute, `impressionDate` has been added to detailed payloads for view-through attribution. A new value has been added to the `claimType` field. See attributionToken(). |
| November, 2024 | The attributionToken() returns a new `claimType` attribute with a value of `Click`, specifying that the app download was from a tap on an ad. Note that the tap-through attribution window is 30 days. |
| May, 2024 | To reduce the rate of delayed attribution responses resulting in 404 errors, the Ad Services API will hold connections for up to 1 second before responding with a 404 error code. Doing this allows more time for the request to be processed and correct data delivered as a part of the response, increasing the number of successful API requests. The impact on the API caller could result in an increased number of client-side connection timeouts in cases if timeout is configured for less than 1 second. |
| March, 2023 | Updated AdServices workflow and attributionToken(). |
| October, 2022 | Updated `adId` in Attribution payload descriptions. |
| January, 2022 | Custom Product Pages replaces Creative Sets functionality.  Apple Search Ads no longer supports Creative Sets and `AdGroupCreativeSets`. Creative Sets API calls return 200 OK responses with an invalid state. Your Creative Sets data remains available through Get Creative Set-Level Reports and through the `AdServices` attribution framework for devices running running iOS versions earlier than 15.2 where `creativeSetId` returns in payloads. For devices running iOS version 15.2 and later, `adId` returns in campaigns using a SupplySource of `APPSTORE_TODAY_TAB` or `APPSTORE_SEARCH_RESULTS.` |

