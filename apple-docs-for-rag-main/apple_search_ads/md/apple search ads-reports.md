

- Apple Search Ads
-  Reports 

API Collection

# Reports

Generate performance metrics for your campaigns.

## Overview

You can fetch reports for campaigns, ad groups, targeting keywords, search terms, and creative sets. See the ReportingRequest object for guidance for setting up your report request payloads.

## Topics

### Reports Endpoints

Get Campaign-Level Reports

Fetches reports for campaigns.

Get Ad Group-Level Reports

Fetches reports for ad groups within a campaign.

Get Keyword-Level Reports

Fetches reports for targeting keywords within a campaign.

Get Keyword-Level within Ad Group Reports

Fetches reports for targeting keywords within an ad group.

Get Search Term-Level Reports

Fetches reports for search terms within a campaign.

Get Search Term-Level within Ad Group Reports

Fetches reports for search terms within an ad group.

Get Ad-Level Reports

Fetches ad performance data within a campaign.

### Reports Request and Response Objects

object ReportingRequest

The report request body.

object ReportingResponseBody

The container object for the report response body.

object ReportingResponse

The container object of report metrics.

object ReportingDataResponse

The total metrics for a report.

object GrandTotalsRow

The summary of cumulative metrics.

object SpendRow

The reporting response metrics.

object ExtendedSpendRow

The descriptions of metrics with dates.

object Row

The report metrics by time granularity.

object ReportingCampaign

The response to a request to fetch campaign-level reports.

object ReportingAdGroup

The response to a request to fetch ad group-level reports.

object ReportingKeyword

The response to a request to fetch keyword-level reports.

object ReportingSearchTerm

The response to a request to fetch search term-level reports.

object ReportingAd

The response to a request to fetch ad-level reports.

object CampaignAppDetail

The app data to fetch from campaign-level reports.

object InsightsObject

The container object for bid recommendations.

object KeywordInsights

The object that contains bid recommendations.

object KeywordBidRecommendation

The suggested bid amount for a keyword.

### Data Types

type MetaDataObject

The report response objects.

## See Also

### Reports

Impression Share Reports

Obtain metrics with impression share insights.

