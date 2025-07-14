

- Analytics Reports
-  Networking Connection Activity 

Article

# Networking Connection Activity

Review how your app uses network connections.

## Overview

The data in this report contains information about your application’s use of network connections. This includes bytes sent and received, and duration of connections.

- Territories: Worldwide

- Platforms: iOS, iPadOS. For more information about iOS and iPadOS, see the Platforms section in Data Completeness and Corrections.

- Availability:

  - Daily: Every day.

- History: On request, data is available beginning with iOS 17.4 and iPadOS 17.4.

- Completeness: Data from devices that contribute to this report can arrive as late as 8 days after the date it generates on device. You can download recent data daily, but it might be incomplete, and data updates incrementally daily, until all late-arriving events are available.

- Privacy:

  - Includes data from users who have opted to share their data with Apple and developers.

  - Individual rows will only appear if they have a value of 5 or more.

- Data Context: You can analyze your data with additional context by comparing it with the data in the App Sessions Context report, which provides a count of unique devices that use your app on a specific day. For example, if your app performed an action detailed in this report on 10 unique devices on a specific day, and the App Sessions Context report shows there were 100 unique devices running your app that day, then you can approximate that 10% of the devices running your app performed that action.

## Report Fields

| Report Field | Description | Data Type |
|----|----|----|
| Count | Number of times the event occurred | `integer` |
| Territory | Country or region in which the event occurred | `string` |
| Date | Date when the event occurred | `string` |
| Platform | OS version on the device on which the event occurred | `string` |
| Device | Type of device on which the event occurred | `string` |
| Build | Build of device on which event occurred | `string` |
| Unique Devices | The count of unique devices | `integer` |
| Release Type | Type of software release | `string` |
| Completion Reason | Network connection completion reason | `string` |
| Download Bytes Bins | Number of bytes, in bins, downloaded during the network connection | `string` |
| Duration In Seconds Bins | Duration in seconds of the network connection | `string` |
| Error | Errors during the network connection | `string` |
| Is Background | Whether the app making the request is in the background when making the network connection call | `boolean` |
| Upload Bytes Bins | Number of bytes, in bins, uploaded during the network connection | `string` |

## Glossary

| Dimension                | Value                | Definition                |
|--------------------------|----------------------|---------------------------|
| Completion Reason        | Success              | Successful completion     |
| Completion Reason        | Failure              | Failure                   |
| Completion Reason        | Cancelled            | Cancelled                 |
| Completion Reason        | None                 | Unknown                   |
| Download Bytes Bins      | \10000000           | Greater than 10MB         |
| Duration In Seconds Bins | \1800               | greater than 1800 seconds |
| Error                    | 0                    | No error                  |
| Error                    | -1001                | CFURL Error timeout       |
| Error                    | Others               | Refer to CFNetworkErrors  |
| Upload Bytes Bins        | \10000000           | Greater than 10MB         |

## See Also

### Performance

AirPlay Errors

Analyze AirPlay errors in your apps.

AirPlay Performance

Review AirPlay performance in your apps.

App Crashes Expanded

Analyze the rate at which your app crashes.

App Installs Performance

Analyze details about installation success and failure rates for your apps.

App Storage Reads and Writes

Analyze how often your app uses disk reads and writes.

Audio Overloads

Analyze how many audio glitches people experience in your app.

Bluetooth LE Session Duration

Analyze how long your app uses Bluetooth Low Energy (LE) connections.

Bluetooth System Wakes

Analyze details about bluetooth system wakes that your app causes.

CAMetalLayer Performance

Review CAMetalLayer metadata and performance in your app.

Custom Language Model Builds Failed

Analyze how often your app-triggered rebuild of a custom language model failed.

Display Power Information

Review your app’s impact on display pixel attributes.

HTTP Live Streaming Playback Errors

Analyze playback errors that your app receives.

Launch Image Over Memory Limit

Analyze how often your app fails to load because it’s over the memory limit.

Spotlight Query Performance

Review how your app uses Spotlight queries.

Streaming Downloads Performance

Review download performance when using the AVAssetDownloadTask APIs in your apps.

