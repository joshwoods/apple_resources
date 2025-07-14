

- Xcode
- Performance and metrics
-  Analyzing the performance of your shipping app 

Article

# Analyzing the performance of your shipping app

View power and performance metrics for apps you distribute through the App Store.

## Overview

Use the Xcode Organizer to view anonymized performance data from your app’s users, including launch times, memory usage, UI responsiveness, and impact on the battery. Use the data to tune the next version of your app and catch regressions that make it into a specific version of your app.

In Xcode, choose Window \> Organizer to open the Organizer window, and then select the desired metric or report. In some cases, the pane shows “Insufficient usage data available” because there may not be enough anonymized data reported from participating user devices. When this happens, try checking back in a few days.

### Read data for a metric

The Xcode Organizer shows a title, description, and graph for each type of metric. In the graph, each bar represents a version of your app. Use the pop-up menus to filter the metric data for different devices and the median or high value. If your app has an App Clip available, use the pop-up menu to filter by app type and switch between viewing metrics for the main app and the App Clip.

Metrics that show *limited usage* in the detail section include an associated margin of error because the existing data is limited. Use this margin of error to determine the upper and lower bounds of the displayed value. The margin of error decreases as data increases. The release date information in this section provides the date when the selected app version is ready for sale.

### Compare performance with a previous app release

To explore changes between versions for a metric, such as those for Hang Rate in the image below, click the vertical bar for your selected version.

The data for both the selected and latest versions appear to the right of the graph with the higher of the two values in bold. Change information for those versions appears in the details section below the latest version data.

### Read data for smart insights

The Xcode Organizer presents a list of smart insights whenever the system detects new performance regressions for the latest version of your app. Each item in the insights list contains information that provides a brief summary.

To the right of the list is the detail pane that shows a chart corresponding to the selected smart insight. Note that the insight for Scroll Hitch Rate for the typical percentile of samples from “iPad (All)” devices is selected. When a selected insight corresponds to more than one percentile, or to different sets of devices, the detail pane presents a scrollable list of additional charts.

To the right of the chart is the insight data showing the metric value for the latest version, as well as the average metric values for the previous four versions. Use this information to see how your latest app version is performing with respect to the average of the previous versions.

Select the Notifications button in the upper-right corner to opt in to power and performance regression notifications. Xcode sends you a notification for the latest version of each of your shipped apps when it detects a high-impact regression. A regression is considered high impact if performance data is available and indicates the latest version of your app regresses 75 percent or more compared to the average of the previous four app versions available in the App Store. Xcode notifies you once per 24-hour period when Xcode is running. To keep notifications to a minimum, Xcode sends you no more than one notification for the same app version.

For more details about how to use the data in the Organizer panes to improve the performance of the next version of your app, see the topics below.

## See Also

### Related Documentation

Analyzing responsiveness issues in your shipping app

Identify responsiveness issues your users encounter, and use the hang and hitch data in Xcode Organizer to determine which issues are most important to fix.

Analyzing your app’s battery use

Increase the available use time for your app on a single battery charge by reducing your appʼs power consumption.

Improving app responsiveness

Create a user experience that feels responsive by removing hangs and hitches from your app.

Reducing disk writes

Improve your app’s responsiveness by optimizing how it writes data to permanent storage.

Reducing your app’s launch time

Create a more responsive experience with your app by minimizing time spent in startup.

Reducing your app’s memory use

Improve your app’s performance by analyzing memory-use metrics and making changes to maximize memory efficiency.

### Essentials

Improving your app’s performance

Model, measure, and boost the performance of your app by using a continuous-improvement cycle.

Profiling apps using Instruments

Use Instruments to analyze the performance, resource usage, and behavior of your apps. Learn how to improve responsiveness, reduce memory usage, and analyze complex behavior over time.

Creating a performance plan for your visionOS app

Identify your app’s performance and power goals and create a plan to measure and assess them.

