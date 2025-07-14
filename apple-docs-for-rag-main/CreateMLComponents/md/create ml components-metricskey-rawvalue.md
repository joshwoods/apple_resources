

- Create ML Components
- MetricsKey
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var rawValue: String
```

## Discussion

A new instance initialized with `rawValue` will be equivalent to this instance. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

let selectedSize = PaperSize.Letter
print(selectedSize.rawValue)
// Prints "Letter"

print(selectedSize == PaperSize(rawValue: selectedSize.rawValue)!)
// Prints "true"
```

## See Also

### Getting the properties

static let source: MetricsKey

A key associated with a temporal stream source (e.g. a file name).

static let trainingAccuracy: MetricsKey

A key associated with a training accuracy metric.

static let trainingError: MetricsKey

A key associated with a training error metric.

static let trainingLoss: MetricsKey

A key associated with a training loss metric.

static let trainingMaximumError: MetricsKey

A key associated with a training maximum error metric.

static let trainingMeanAveragePrecision: MetricsKey

A key associated with a training mean average precision metric.

static let validationAccuracy: MetricsKey

A key associated with a validation accuracy metric.

static let validationError: MetricsKey

A key associated with a validation error metric.

static let validationLoss: MetricsKey

A key associated with a validation loss metric.

static let validationMaximumError: MetricsKey

A key associated with a validation maximum error metric.

static let validationMeanAveragePrecision: MetricsKey

A key associated with a validation mean average precision metric.

