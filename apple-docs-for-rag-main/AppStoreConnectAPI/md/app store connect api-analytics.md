

- App Store Connect API
-  Analytics 

API Collection

# Analytics

Get data about your apps and usage.

## Overview

Use the Analytics Reports API to analyze your app’s performance on iOS and the App Store and find opportunities for improvement. To learn more about interpreting the data using the glossary of report fields and definitions, see Analytics Reports.

To help protect user privacy, where appropriate, Apple is applying measures to protect personally identifable infomation. For specific reports, Apple adds noise or applies crowd anonymity, and uses both approaches for other reports. Apple only reports totals when a specific number of data points are available. For more infomation about these measures, see Protecting user privacy in report data.

To download analytics reports, be sure you have one of the following user roles:

- ADMIN

- SALES AND REPORTS

- FINANCE

This table outlines which roles can use which resources:

| Role | Manage requests | List and download reports |
|----|----|----|
| Admin | Request reports and Delete a report request | Read reports for a specific request |
| Finance |  | Read reports for a specific request |
| Sales and Reports |  | Read reports for a specific request |

The Sales and Reports role can also read Download Sales and Trends Reports in addition to Analytics Reports.

To learn more about roles, see Program Roles.

Note

If you have any questions about the data made available in this API, including about how Apple applies privacy measures to protect user privacy and complies with legal obligations, contact Apple through Feedback Assistant by selecting the following option:

Developer Tools & Resources \> App Store Connect API \> Data Request

Learn more about how to use Feedback Assistant.

## Topics

### Essentials

Downloading Analytics Reports

Learn how to request and review data about your apps, their usage, engagement, and performance.

### Making, Reading, and Deleting Requests

Request reports

Request analytics reports for your apps.

Read report requests

Read analytics report requests for a specific app.

Read report request information

Get details for and the state of a specific analytics report request.

Read reports for a specific request

Get a list of reports generated from a specific analytics report request.

Delete a report request

Remove a specific analytics report request.

### Reading Reports, Instances, and Segments

Read report information

Get details for a specific analytics report.

Read a list of instances of a report

Read list of all the granularity options for a specific type of analytics report.

Read report instance information

Get details for a specific instance of an analytics report.

Read the segments for a report

Get details for a specific analytics report segment.

Read the details for a report segment

Get details and download information for a specific analytics report segment.

### Objects

object AnalyticsReportRequest

The data structure that represents an analytics report request.

object AnalyticsReportRequestCreateRequest

The request body you use to create an analytics report request.

object AnalyticsReportRequestResponse

A response that contains a single analytics report request resource.

object AnalyticsReportRequestsResponse

A response that contains a list of analytics report request resources.

object AnalyticsReport

The data structure that represents an analytics report.

object AnalyticsReportResponse

A response that contains a single analytics report resource.

object AnalyticsReportsResponse

A response that contains a list of analytics report resources.

object AnalyticsReportInstance

The data structure that represents an analytics report instance.

object AnalyticsReportInstanceResponse

A response that contains a single analytics report instance resource.

object AnalyticsReportInstancesResponse

A response that contains a list of analytics report instance resources.

object AnalyticsReportSegment

The data structure that represents an analytics report segment.

object AnalyticsReportSegmentResponse

A response that contains a single analytics report segment resource.

object AnalyticsReportSegmentsResponse

A response that contains a list of analytics report segment resources.

## See Also

### Reporting

Sales and Finance

Download your sales and financial reports.

Power and Performance Metrics and Logs

Get power and performance metrics, logs, and signatures.

