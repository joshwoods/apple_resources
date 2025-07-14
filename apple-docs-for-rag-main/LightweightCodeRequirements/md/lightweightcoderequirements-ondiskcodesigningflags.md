

- LightweightCodeRequirements
-  OnDiskCodeSigningFlags 

Structure

# OnDiskCodeSigningFlags

A constraint that tests the code-signing flags of a code file on disk.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct OnDiskCodeSigningFlags
```

## Topics

### Structures

struct ValueSet

Code signing flags that can be set on code on disk.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias DataType

The basic input data type for this constraint: `OnDiskCodeSigningFlags.ValueSet`

typealias OutType

The type of this constraint: OnDiskCodeSigningFlags

### Type Methods

static func isSuperset(of: OnDiskCodeSigningFlags.DataType) -> OnDiskCodeSigningFlags.OutType

Matches when the code signing flags on the file/slice are a superset of the specified flags.

## Relationships

### Conforms To

- Decodable
- Encodable
- OnDiskConstraint
- Sendable

## See Also

### Checking code requirements for code files on disk

func SecStaticCodeCheckValidityWithOnDiskRequirement(code: SecStaticCode, flags: SecCSFlags, requirement: OnDiskCodeRequirement) -> ValidationResult

Checks whether static code on disk satisfies a lightweight code requirement.

func SecCodeCheckValidityWithOnDiskRequirement(code: SecCode, flags: SecCSFlags, requirement: OnDiskCodeRequirement) -> ValidationResult

Checks whether code on disk satisfies a lightweight code requirement.

struct ValidationResult

A structure that represents the result of testing a lightweight code requirement.

struct OnDiskCodeRequirement

A lightweight code requirement that you use to evaluate a code file on disk.

func allOf(requirement: () -> [any OnDiskConstraint]) -> any OnDiskConstraint

Creates a constraint that requires code on disk to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any OnDiskConstraint]) -> any OnDiskConstraint

Creates a constraint that requires code on disk to satisfy any of the provided constraints.

protocol OnDiskConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in on-disk code requirements.

struct OnDiskConstraintBuilder

A custom parameter attribute that constructs on-disk constraints from closures.

