

- Exposure Notification
- ENManager
-  getExposureInfo(summary:userExplanation:completionHandler:) Deprecated

Instance Method

# getExposureInfo(summary:userExplanation:completionHandler:)

Returns information about each exposure.

iOS 13.5–13.6DeprecatediPadOS 13.5–13.6DeprecatedMac Catalyst 13.5–13.6Deprecated

``` source
func getExposureInfo(
    summary: ENExposureDetectionSummary,
    userExplanation: String,
    completionHandler: @escaping ENGetExposureInfoHandler
) -> Progress
```

Deprecated

Use getExposureWindowsFromSummary, if needed.

## Parameters 

`summary`  

The summary of exposure.

`userExplanation`  

A string that the framework displays to the user informing them of the exposure.

`completionHandler`  

The completion handler that the framework calls when the method completes.

## Return Value

The progress of the method.

## Discussion

Important

This method is available in iOS 12.5, and in iOS 13.5 to 13.6.

Calls to this method generate a user notification that presents the `userExplanation`.

## Topics

### Completion Handlers

typealias ENGetExposureInfoHandler

The definition of a handler that receives exposure info.

## See Also

### Obtaining Exposure Information

func detectExposures(configuration: ENExposureConfiguration, diagnosisKeyURLs: [URL], completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the configuration that you specify for controlling the scoring algorithm.

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

