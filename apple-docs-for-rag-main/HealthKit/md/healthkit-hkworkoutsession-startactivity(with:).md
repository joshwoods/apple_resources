

- HealthKit
- HKWorkoutSession
-  startActivity(with:) 

Instance Method

# startActivity(with:)

Starts the workout session activity, and sets the start date.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 5.0+

``` source
func startActivity(with date: Date?)
```

## Parameters 

`date`  

The start date for the workout session.

## See Also

### Related Documentation

case running

The workout session is running.

### Managing the workout

func prepare()

Prepares the workout session.

func pause()

Pauses the workout session.

func resume()

Resumes the workout session.

func stopActivity(with: Date?)

Stops the workout session activity, and sets the end date.

func end()

Ends the workout session.

