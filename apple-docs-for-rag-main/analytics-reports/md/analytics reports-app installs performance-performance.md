

- Analytics Reports
-  App Installs Performance 

Article

# App Installs Performance

Analyze details about installation success and failure rates for your apps.

## Overview

Use this report to help you understand your app’s installation success and failure rates.

- Territories: Worldwide

- Platforms: iOS, iPadOS, macOS, tvOS, visionOS

- Availability:

  - Daily: Every day

- History: On request, data is available beginning from March 1, 2024.

- Completeness: Within two days.

- Privacy: Includes data from users who have opted to share their data with Apple and developers. Data is provided only when events exist from at least five users for the respective report.

The Analytics Reports framework delivers new portions of report content as instances. Each instance can contain one or more batches of data, to accommodate late-arriving events, or in rare cases, data corrections. To learn more, see Data Completeness and Corrections.

## Report Fields

| Report Field | Description | Data Type |
|----|----|----|
| Date | Date on which the event occurred. For weekly and monthly instances, this column represents the first day of the week and month, respectively. | `date` |
| App Name | The name of the app provided by you during app setup in App Store Connect. | `string` |
| App Apple Identifier | Your app’s Apple ID. | `integer` |
| Download Type | The type of download or install. | `string` |
| Download Info | Additional context on the type of download or install. | `string` |
| Install Status | Indicates if the app install succeed or failed | `string` |
| Install Package Type | Type of install package | `string` |
| Device | Type of device on which the event occurred | `string` |
| Platform Version | OS version on the device on which the event occurred | `string` |
| Territory | App Store country in which the event occurred | `string` |
| Counts | Aggregated count of events | `integer` |
| Avg Install Duration | Average time in milliseconds taken to install the package | `integer` |

## Glossary

| Dimension | Value | Definition |
|----|----|----|
| Download Type | First-time downloads | Your app was downloaded on the device for the first-time by the user |
| Download Type | Redownloads | Your app was re-downloaded on the device by the user |
| Download Type | Updates | Your app was updated by the user |
| Download Type | Auto-update | Your app was auto-updated on the user’s device. |
| Download Type | Restores | Your app was restored from a backup on a new or newly erased device |
| Download Type | Auto-downloads | Your app was auto-downloaded to the user’s device. |
| Download Type | App Clip installs | Your App Clip was installed on the user’s device |
| Download Info | Code redemption | The user redeemed an offer code for your app. |
| Download Info | Pre-order | Your app that was pre-ordered was downloaded onto the user’s device. |
| Download Info | Preloaded | Your app was preloaded onto the user’s device. |
| Download Info | TestFlight | Your app was downloaded onto the user’s device from TestFlight. |
| Download Info | Alternative app marketplace | Your app was distributed to the user outside the App Store. |

## See Also

### Performance

AirPlay Errors

Analyze AirPlay errors in your apps.

AirPlay Performance

Review AirPlay performance in your apps.

App Crashes Expanded

Analyze the rate at which your app crashes.

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

Networking Connection Activity

Review how your app uses network connections.

Spotlight Query Performance

Review how your app uses Spotlight queries.

Streaming Downloads Performance

Review download performance when using the AVAssetDownloadTask APIs in your apps.

