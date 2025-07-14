

- HealthKit
-  HKWorkoutActivityType 

Enumeration

# HKWorkoutActivityType

The type of activity performed during a workout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKWorkoutActivityType
```

## Mentioned in 

Dividing a HealthKit workout into activities

## Topics

### Individual sports

case archery

The constant for shooting archery.

case bowling

The constant for bowling.

case fencing

The constant for fencing.

case gymnastics

Performing gymnastics.

case trackAndField

Participating in track and field events, including shot put, javelin, pole vaulting, and related sports.

### Team sports

case americanFootball

The constant for playing American football.

case australianFootball

The constant for playing Australian football.

case baseball

The constant for playing baseball.

case basketball

The constant for playing basketball.

case cricket

The constant for playing cricket.

case discSports

The constant for playing disc sports such as Ultimate and Disc Golf.

case handball

The constant for playing handball.

case hockey

The constant for playing hockey, including ice hockey, field hockey, and related sports.

case lacrosse

The constant for playing lacrosse.

case rugby

The constant for playing rugby.

case soccer

The constant for playing soccer.

case softball

The constant for playing softball.

case volleyball

The constant for playing volleyball.

### Exercise and fitness

case preparationAndRecovery

The constant for warm-up and therapeutic activities like foam rolling and stretching.

case flexibility

The constant for a flexibility workout.

case cooldown

The constant for low intensity stretching and mobility exercises following a more vigorous workout.

case walking

The constant for walking.

case running

The constant for running and jogging.

case wheelchairWalkPace

The constant for a wheelchair workout at walking pace.

case wheelchairRunPace

The constant for wheelchair workout at running pace.

case cycling

The constant for cycling.

case handCycling

The constant for hand cycling.

case coreTraining

The constant for core training.

case elliptical

The constant for workouts on an elliptical machine.

case functionalStrengthTraining

The constant for strength training, primarily with free weights and body weight.

case traditionalStrengthTraining

The constant for strength training exercises primarily using machines or free weights.

case crossTraining

The constant for exercise that includes any mixture of cardio, strength, and/or flexibility training.

case mixedCardio

The constant for workouts that mix a variety of cardio exercise machines or modalities.

case highIntensityIntervalTraining

The constant for high intensity interval training.

case jumpRope

The constant for jumping rope.

case stairClimbing

The constant for workouts using a stair climbing machine.

case stairs

The constant for running, walking, or other drills using stairs (for example, in a stadium or inside a multilevel building).

case stepTraining

The constant for training using a step bench.

case fitnessGaming

The constant for playing fitness-based video games.

### Studio activities

case barre

The constant for barre workout.

case cardioDance

The constant for cardiovascular dance workouts.

case socialDance

The constant for dancing with a partner or partners, such as swing, salsa, or folk dances.

case yoga

The constant for practicing yoga.

case mindAndBody

The constant for performing activities like walking meditation, Gyrotonic exercise, and Qigong.

case pilates

The constant for a pilates workout.

### Racket sports

case badminton

The constant for playing badminton.

case pickleball

The constant for playing pickleball.

case racquetball

The constant for playing racquetball.

case squash

The constant for playing squash.

case tableTennis

The constant for playing table tennis.

case tennis

The constant for playing tennis.

### Outdoor activities

case climbing

The constant for climbing.

case equestrianSports

The constant for activities that involve riding a horse, including polo, horse racing, and horse riding.

case fishing

The constant for fishing.

case golf

The constant for playing golf.

case hiking

The constant for hiking.

case hunting

The constant for hunting.

case play

The constant for play-based activities like tag, dodgeball, hopscotch, tetherball, and playing on a jungle gym.

### Snow and ice sports

case crossCountrySkiing

The constant for cross country skiing.

case curling

The constant for curling.

case downhillSkiing

The constant for downhill skiing.

case snowSports

The constant for a variety of snow sports, including sledding, snowmobiling, or building a snowman.

case snowboarding

The constant for snowboarding.

case skatingSports

The constant for skating activities, including ice skating, speed skating, inline skating, and skateboarding.

### Water activities

case paddleSports

The constant for canoeing, kayaking, paddling an outrigger, paddling a stand-up paddle board, and related sports.

case rowing

The constant for rowing.

case sailing

The constant for sailing.

case surfingSports

The constant for a variety of surf sports, including surfing, kite surfing, and wind surfing.

case swimming

The constant for swimming.

case waterFitness

The constant for aerobic exercise performed in shallow water.

case waterPolo

The constant for playing water polo.

case waterSports

The constant for a variety of water sports, including water skiing, wake boarding, and related activities.

### Martial arts

case boxing

The constant for boxing.

case kickboxing

The constant for kickboxing.

case martialArts

The constant for practicing martial arts.

case taiChi

The constant for tai chi.

case wrestling

The constant for wrestling.

### Other activities

case other

The constant for a workout that does not match any of the other workout activity types.

### Deprecated activity types

case dance

The constant for dancing.

Deprecated

case danceInspiredTraining

The constant for workouts inspired by dance, including Pilates, Barre, and Feldenkrais.

Deprecated

case mixedMetabolicCardioTraining

The constant for performing any mix of cardio-focused exercises.

Deprecated

### Multisport activities

case swimBikeRun

The constant for multisport activities like triathlons.

case transition

A constant for the transition time between activities in a multisport workout.

### Enumeration Cases

case underwaterDiving

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Samples

Adding samples to a workout

Create associated samples that add details to a workout.

Accessing condensed workout samples

Read series data from condensed workouts.

Dividing a HealthKit workout into activities

Partition multisport and interval workouts into activities that represent the different parts of the workout.

class HKWorkout

A workout sample that stores information about a single physical activity.

class HKWorkoutActivity

An object that describes an activity within a longer workout.

class HKWorkoutBuilder

A builder object that incrementally constructs a workout.

class HKWorkoutType

A type that identifies samples that store information about a workout.

let HKWorkoutTypeIdentifier: String

The workout type identifier.

enum HKWorkoutSessionType

The type of session.

class HKWorkoutEvent

An object representing an important event during a workout.

