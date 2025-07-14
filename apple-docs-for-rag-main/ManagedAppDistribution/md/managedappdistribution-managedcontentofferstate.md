

- ManagedAppDistribution
-  ManagedContentOfferState 

Structure

# ManagedContentOfferState

ManagedAppDistributionSwiftUIiOS 17.2+iPadOS 17.2+

``` source
struct ManagedContentOfferState
```

## Topics

### Creating states

static func custom(title: String) -> ManagedContentOfferState

A state with a custom title.

static func installing(progress: Double?) -> ManagedContentOfferState

A state indicating install progress.

### Determining installation status

static var installed: ManagedContentOfferState

A state representing content that’s installed.

static var notInstalled: ManagedContentOfferState

A state for representing content that isn’t currently installed.

static var neverInstalled: ManagedContentOfferState

A state representing content that has never been installed.

static var noninteractive: ManagedContentOfferState

A state representing content that has no actionable button.

### Operators

static func == (ManagedContentOfferState, ManagedContentOfferState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### View creation

struct ManagedAppView

A view that displays a managed app.

struct ManagedContentView

struct ManagedContentStyle

A type that applies a custom appearance to the managed content view.

