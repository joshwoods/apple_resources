

- Exposure Notification
- ENManager
-  detectExposures(configuration:diagnosisKeyURLs:completionHandler:) 

Instance Method

# detectExposures(configuration:diagnosisKeyURLs:completionHandler:)

Detects exposures using the configuration that you specify for controlling the scoring algorithm.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
func detectExposures(
    configuration: ENExposureConfiguration,
    diagnosisKeyURLs: [URL],
    completionHandler: @escaping ENDetectExposuresHandler
) -> Progress
```

## Parameters 

`configuration`  

The configuration to use for scoring.

`diagnosisKeyURLs`  

An array of file URLs that contain downloaded diagnosis keys.

`completionHandler`  

The completion handler that the framework calls when the method completes.

## Return Value

The progress of the method.

## Discussion

Important

This method is available in iOS 12.5, and in iOS 13.5 and later.

The `diagnosisKeyURLs` parameter requires an array of file URLs that point to exposure key data files downloaded from an exposure notification (EN) server. For more information about the data format used to transmit diagnosis key data, see Setting Up a Key Server.

When you retrieve diagnosis key data from an EN server, you receive it as a zip archive that you must decompress before use. Every archive you download from an EN server includes two files with the same base name, but with different file extensions: a key file with a `.bin` extension, and a signature file with a `.sig` extension. Decompress both files in the same directory, create a URL that points to each of the extracted files, and then pass both URLs as an array to `diagnosisKeyURLs` argument in an array.

If a diagnosis key has a rolling period greater than 144, the framework ignores it and will not consider it for key matching.

You may submit multiple file pairs in a single call to this method; however, each pair must use a unique base name. The order of the URLs passed in the `diagnosisKeyURLs` array doesn’t matter. The file pairs will be matched up using the base name.

On iOS 13.7 and later, exposure keys that you submit to this method are automatically cached and used by the EN framework in calculations for up to 14 days. If you want to recalculate an ERV using different configuration values, use detectExposures(configuration:completionHandler:) to recalculate a new ERV using only cached exposure keys.

Important

On iOS 13.6 and later, you’re limited to using this method a maximum of 15 times per 24-hour period. If you’re on iOS 13.7 and later and specify `2` as the `ENAPIVersion` in your app’s `Info.plist` file, you’re limited to using this method a maximum of 6 times per 24-hour period.

On iOS 13.5, you can only submit 15 uncached key files per 24-hour period, regardless of the number of API calls you make.

### Log Exposures

ExposureNotification provides transparency for users at several points. For example, a user can choose Settings \> Exposure Notifications to show the status of COVID-19 Exposure Logging, along with the currently active app, and its activity. This activity view shows the number of diagnostic key checks in the past 14 days, and the hash of the checked sets of keys.

To export the exposure checks, tap Export Exposure Checks. The resulting JSON file contains a `Files` array.

```
```

Within the array are several properties, including the timestamp of the check (`Timestamp`), and how many positive keys the device downloaded and checked on the device (`KeyCount`) at that time.

iOS also provides a monthly notification to the user that reads, “Your iPhone continues to look for possible exposures on your behalf.” The notification occurs if the user has installed an EN app and enabled Exposure Logging, and the app has run a check for matched keys. The notification ensures that the app doesn’t continue to share proximity events without notifying the user. Users who tap the notification arrive at the transparency details in the Settings app, as described earlier.

## Topics

### Completion Handlers

typealias ENDetectExposuresHandler

The definition of a handler that returns exposure summaries.

## See Also

### Obtaining Exposure Information

func detectExposures(configuration: ENExposureConfiguration, completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the specified configuration to control the scoring algorithm.

func getExposureWindows(summary: ENExposureDetectionSummary, completionHandler: ENGetExposureWindowsHandler) -> Progress

Obtains information from the provided summary about the user’s exposure within a window of time.

typealias ENGetExposureWindowsHandler

The handler the system invokes when the acquisition of windows completes.

func getUserTraveled(completionHandler: ENGetUserTraveledHandler)

Obtains information about the user’s travel within an exposure period.

typealias ENGetUserTraveledHandler

The handler the system invokes when acquistiion of the user’s travel status completes.

func getExposureInfo(summary: ENExposureDetectionSummary, userExplanation: String, completionHandler: ENGetExposureInfoHandler) -> Progress

Returns information about each exposure.

Deprecated

