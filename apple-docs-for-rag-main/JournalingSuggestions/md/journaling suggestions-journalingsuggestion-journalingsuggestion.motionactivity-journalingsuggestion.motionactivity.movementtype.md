

- Journaling Suggestions
- JournalingSuggestion
- JournalingSuggestion.MotionActivity
-  JournalingSuggestion.MotionActivity.MovementType 

Structure

# JournalingSuggestion.MotionActivity.MovementType

The movement activity type that the phone records when it detects motion.

iOS 18.0+

``` source
struct MovementType
```

## Topics

### Recording movement type

static let running: JournalingSuggestion.MotionActivity.MovementType

A running movement activity type.

static let runningWalking: JournalingSuggestion.MotionActivity.MovementType

A mixed running and walking movement activity type.

static let walking: JournalingSuggestion.MotionActivity.MovementType

A walking movement activity type.

### Decoding a value

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Operators

static func == (JournalingSuggestion.MotionActivity.MovementType, JournalingSuggestion.MotionActivity.MovementType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable

## See Also

### Inspecting motion details

var steps: Int

The number of steps a person takes.

var movementType: JournalingSuggestion.MotionActivity.MovementType?

The specific type of movement associated with the activity.

