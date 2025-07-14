

- Exposure Notification
-  ENGetExposureWindowsHandler 

Type Alias

# ENGetExposureWindowsHandler

The handler the system invokes when the acquisition of windows completes.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
typealias ENGetExposureWindowsHandler = ([ENExposureWindow]?, (any Error)?) -> Void
```

## Parameters 

`exposureWindows`  

An array of available exposure windows. The contents of this array are in no particular order.

`error`  

A successful invocation if `nil`; otherwise, the error that occured.

## Discussion

Important

This type is available in iOS 12.5, and in iOS 13.5 and later.

## See Also

### Obtaining Exposure Information

func detectExposures(configuration: ENExposureConfiguration, diagnosisKeyURLs: [URL], completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the configuration that you specify for controlling the scoring algorithm.

func detectExposures(configuration: ENExposureConfiguration, completionHandler: ENDetectExposuresHandler) -> Progress

Detects exposures using the specified configuration to control the scoring algorithm.

func getExposureWindows(summary: ENExposureDetectionSummary, completionHandler: ENGetExposureWindowsHandler) -> Progress

Obtains information from the provided summary about the user’s exposure within a window of time.

func getUserTraveled(completionHandler: ENGetUserTraveledHandler)

Obtains information about the user’s travel within an exposure period.

typealias ENGetUserTraveledHandler

The handler the system invokes when acquistiion of the user’s travel status completes.

func getExposureInfo(summary: ENExposureDetectionSummary, userExplanation: String, completionHandler: ENGetExposureInfoHandler) -> Progress

Returns information about each exposure.

Deprecated

