

- App Intents
-  RelevantContext 

Structure

# RelevantContext

A type that specifies conditions for relevance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct RelevantContext
```

## Topics

### Structures

struct FitnessCondition

struct HeadphonesCondition

struct InferredLocation

struct SleepCondition

### Type Methods

static func date(Date) -> RelevantContext

An exact point in time, such as the start of a sporting event or a live broadcast.

static func date(from: Date, to: Date) -> RelevantContext

An exact range in time: similar uses as `date()`, but with a known endpoint.

static func fitness(RelevantContext.FitnessCondition) -> RelevantContext

Fitness.

static func hardware(headphones: RelevantContext.HeadphonesCondition) -> RelevantContext

Hardware

static func location(CLRegion) -> RelevantContext

An exact region. To create a region based on a point location or an address, see CoreLocation.

static func location(inferred: RelevantContext.InferredLocation) -> RelevantContext

An abstract location, inferred from user behavior.

static func sleep(RelevantContext.SleepCondition) -> RelevantContext

Sleep

## See Also

### Intent relevancy

struct RelevantIntent

A type that specifies an intent and its relevance to the user.

class RelevantIntentManager

A type that saves relevant intents.

