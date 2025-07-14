

- Core Motion
-  CMMovementDisorderManager 

Class

# CMMovementDisorderManager

A manager for recording and querying movement disorder data.

watchOS 5.0+

``` source
class CMMovementDisorderManager
```

## Mentioned in 

Getting movement disorder symptom data

## Overview

Important

Only collect data from patients clinically diagnosed with a movement disorder. This API is not designed to collect data from users who have not been diagnosed with a movement disorder. All medical decisions should be made through the guidance of a licensed clinician. For more information, see Adhering to the movement disorder data collection requirements.

Use `CMMovementDisorderManager` to measure a resting Parkinsonian tremor in the 3-7 Hz range and choreiform dyskinetic symptoms. When collecting data, the user should wear Apple Watch on their most affected arm.

`CMMovementDisorderManager` requires an entitlement from Apple. To apply for the entitlement, see Movement Disorder Entitlement Request.

Important

To use this API, you must include the NSMotionUsageDescription key in your app’s `Info.plist` file and provide a usage description string for this key. The usage description appears in the prompt that the user must accept the first time the system asks the user to access motion data for your app. If you don’t include a usage description string, your app crashes when you call this API.

## Topics

### Checking Availablility

class func isAvailable() -> Bool

A Boolean value indicating whether the current device supports the movement disorder manager.

class func authorizationStatus() -> CMAuthorizationStatus

A value indicating whether the user has authorized the app to monitor and query for movement disorder data.

class func version() -> String?

Returns a string that describes the movement disorder algorithm’s current version.

### Recording Movement Disorders

func monitorKinesias(forDuration: TimeInterval)

Calculate and store tremor and dyskinetic symptom results for the duration of the specified time interval.

func monitorKinesiasExpirationDate() -> Date?

Returns the expiration date for the most recent monitoring period.

### Querying for Movement Disorders

func queryTremor(from: Date, to: Date, withHandler: CMTremorResultHandler)

Query for tremor results from the provided time interval.

typealias CMTremorResultHandler

A completion handler for accessing and processing tremor results.

func queryDyskineticSymptom(from: Date, to: Date, withHandler: CMDyskineticSymptomResultHandler)

Query for dyskinetic symptoms from the provided time interval.

typealias CMDyskineticSymptomResultHandler

A completion handler for processing dyskinetic symptom results.

func lastProcessedDate() -> Date?

Returns the date of the most recently calculated results.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Movement disorder

Getting movement disorder symptom data

Retrieve data from the Apple Watch’s movement disorder manager.

Adhering to the movement disorder data collection requirements

Ensure that your users understand and have control over the data your app collects.

Movement disorder algorithm changelog

A chronological log of notable changes to the movement disorder algorithm.

class CMTremorResult

A result object that contains data about the presence and strength of tremors during a one-minute interval.

class CMDyskineticSymptomResult

A result object that contains data about the likely presence of dyskinetic symptoms during a one-minute interval.

