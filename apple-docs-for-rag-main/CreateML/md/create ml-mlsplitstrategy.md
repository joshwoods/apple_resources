

- Create ML
-  MLSplitStrategy 

Enumeration

# MLSplitStrategy

Data partitioning approaches, typically for creating a validation dataset from a training dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
enum MLSplitStrategy
```

## Topics

### Partitioning data

case automatic

Create ML automatically decides how much of your training dataset it uses for a validation dataset.

case fixed(ratio: Double, seed: Int?)

Create ML uses a portion of your training dataset to create a validation dataset based on the ratio.

func resolve(count: Int) -> (ratio: Double, seed: Int)

Resolves this split strategy for a specific element count.

### Creating a random seed

func timestampSeed() -> Int

Creates a deterministic number from the current system time to seed random-number generators.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting Types

enum MLCreateError

The errors Create ML throws while performing various operations, such as training models, making predictions, writing models to a file system, and so on.

struct MLModelMetadata

Information about a model that’s stored in a Core ML model file.

