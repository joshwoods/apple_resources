

- Apple Search Ads
-  Impression Share Reports 

API Collection

# Impression Share Reports

Obtain metrics with impression share insights.

## Overview

Impression share reports provide insights into opportunities to scale keywords and optimize maximum CPT bids and budgets for your search results campaigns. The reports also show you how your app ranks in terms of impression share compared to other apps in the same countries and regions.

Use the Impression Share Report endpoint to obtain a report `ID` to use with Get a Single Impression Share Report, or use Get All Impression Share Reports without a report `ID`.

Use CustomReportRequest for formatting guidance on selector structure. For metrics descriptions, see CustomReportResponse.

## Topics

### Impression Share Report Endpoints

Impression Share Report

Obtain a report ID.

Get a Single Impression Share Report

Fetches a single Impression Share report containing metrics and metadata.

Get All Impression Share Reports

Fetches all Impression Share reports containing metrics and metadata.

### Impression Share Report Request and Response Objects

object CustomReportRequest

The Impression Share report request body.

object CustomReportResponse

A container for Impression Share report metrics.

object CustomReportResponseBody

A container for the Impression Share report response body.

object SovCondition

The list of condition objects that allow users to filter a list of records.

## See Also

### Reports

Reports

Generate performance metrics for your campaigns.

