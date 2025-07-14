

- Analytics Reports
-  Browser Choice Screen Selection 

Article

# Browser Choice Screen Selection

This report details percentage of devices that had your web browser application selected as default from the Browser Choice screen.

## Overview

The data in this report provides details about users’ selection of a default web browser from the browser choice screen. Use this report to understand your browser’s performance on the choice screen.

- Territories: European Union (EU) only.

- Platforms: iOS, iPadOS. For more information about iOS and iPadOS, see the Platforms section in Data Completeness and Corrections.

- Availability:

  - Daily: Every day.

- History: On request, data is available beginning with iOS 18.2 and iPadOS 18.2.

- Completeness: Data from devices that contribute to this report can arrive as late as 8 days after the date it generates on device. You can download recent data daily, but it might be incomplete, and data updates incrementally daily, until all late-arriving events are available.

- Privacy:

  - Includes data from users who have opted to share their data with Apple and developers.

- Data Context: The data in this report provides information about the browser choice screen made available on iOS 18.2+ and iPadOS 18.2+. An older version of the browser choice screen is available on iOS releases prior to 18.2. Data about your web browser app’s performance on the old version of the browser choice screen can be found in the Browser Choice Screen Engagement (iOS versions before 18.2).

## Report Fields

| Report Field | Description | Data Type |
|----|----|----|
| Territory | The user’s region code as set in Settings \> General \> Language & Region. This may not correspond to the user’s Apple Account or App Store storefront. | `string` |
| Date | Date when the event occurred | `string` |
| Platform | OS version on the device on which the event occurred | `string` |
| Device | Type of device on which the event occurred | `string` |
| Build | Build of device on which event occurred | `string` |
| Release Type | Type of software release | `string` |
| Selection Rate | Percentage of unique devices that set your browser app as default among all unique devices that chose a default | `float` |
| New Install Rate | Percentage of unique devices that set your browser app as default without having it installed already, among all unique devices that chose your browser app as a default | `float` |
| Existing Install Rate | Percentage of unique devices that set your browser app as default and already had it installed, among all unique devices that chose your browser app as a default | `float` |
| Product Page Conversion Rate | Percentage of unique devices that set your browser app as default after viewing its product page, among all unique devices that viewed your browser app’s product page | `float` |
| Informed Selection Rate | Percentage of unique devices that set your browser app as default that had previously viewed its product page, among all unique devices that chose your browser app as a default | `float` |
| Direct Selection Rate | Percentage of unique devices that set your browser app as default without viewing its product page, among all unique devices that chose your browser app as a default | `float` |

## See Also

### Framework Usage

AccessorySetupKit Accessory Picker Sessions

Analyze how many people use your app to set up accessories by using AccessorySetupKit.

AccessorySetupKit Usage

Analyze how often your app uses AccessorySetupKit.

AirPlay Discovery Sessions

Review information about AirPlay discovery sessions.

Animoji Stickers Sent

Analyze how many times people use Memoji stickers in your app.

App Added to Focus

Review information about your app’s relationship to Focus modes.

App Disk Space Usage

Analyze your app’s disk space use.

App Runtime Usage

Analyze how often your app executes specific symbols of different dynamic libraries.

App Sessions Context

Analyze how many people use your app and for how long.

Application Preferred Language Settings

Review how people use language preference settings in your app.

ARKit ARSession Duration

Review information about ARKit ARSession duration.

ARKit ARSession Failures

Analyze details about ARKit ARSession failures.

ARKit Capture Frame Rate Throttling

Analyze how long it takes for ARKit to throttle the camera frame rate.

ARKit Collaborative Session Features

Review how your app uses ARKit collaborative session features.

ARKit Face Tracking

Analyze how often your app uses ARKit face tracking.

ARKit Video Formats

Review information about ARKit video formats and high-resolution frames.

