

- HealthKit
- HKWorkoutSession
-  stopActivity(with:) 

Instance Method

# stopActivity(with:)

Stops the workout session activity, and sets the end date.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 5.0+

``` source
func stopActivity(with date: Date?)
```

## Parameters 

`date`  

The end date for the workout session. This must be equal to or after the start date.

## See Also

### Related Documentation

case stopped

The session has stopped.

### Managing the workout

func prepare()

Prepares the workout session.

func startActivity(with: Date?)

Starts the workout session activity, and sets the start date.

func pause()

Pauses the workout session.

func resume()

Resumes the workout session.

func end()

Ends the workout session.

