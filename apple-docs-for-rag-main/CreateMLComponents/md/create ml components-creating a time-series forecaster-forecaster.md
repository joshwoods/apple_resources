

- Create ML Components
-  Creating a time-series forecaster 

Article

# Creating a time-series forecaster

Forecast future data points by training a machine learning model using historical data.

## Overview

Some signals have patterns that repeat over time or have clear trends. For example, the energy consumption of a city has a pattern with peaks in the evening when most people get home. It’s common practice to refer to these signals as time-series data. Other examples of time-series data are:

- The accelerometer on your phone when performing an action.

- The temperature of a machine in a factory.

- Your heart rate during a gym session.

Even though there are patterns to the data, these patterns aren’t trivial to forecast. You can perform forecasts on these data by training an ML model. For example, you can forecast future energy consumption based on historical consumption.

Training a time-series forecaster with the Create ML Components framework shares common training behavior with other model types.

### Prepare your training data

The first step to begin forecasting the energy consumption is to prepare the data. Gather the data as a CSV file, using the following structure:

| Date                | Consumption |
|---------------------|-------------|
| 2024-04-01 00:00:00 | 1.948       |
| 2024-04-01 01:00:00 | 1.678       |
| 2024-04-01 02:00:00 | 1.873       |
| 2024-04-01 03:00:00 | 1.604       |

The table shows a energy consumption reading for every hour (in GWh). Use the date and time because the consumption depends on the season and the time of day. Parse the date string into a `Date` type by using `CSVReadingOptions` and `Date.ParseStrategy`:

```
var options = CSVReadingOptions()
options.floatingPointType = .float
options.addDateParseStrategy(
    Date.ParseStrategy(
        format: "\(year: .defaultDigits)-\(month: .twoDigits)-\(day: .twoDigits) \(hour: .twoDigits(clock: .twentyFourHour, hourCycle: .zeroBased)):\(minute: .twoDigits):\(second: .twoDigits))",
        locale: Locale(identifier: "en_US"),
        timeZone: TimeZone(abbreviation: "GMT")!
    )
)
let dataFrame = try DataFrame(contentsOfCSVFile: url, columns: ["Date", "Temp"], types: ["Date": .date], options: options)
```

Now that you have a data frame with a `Date` column and a `Float` column, create a preprocessing pipeline. First, scale the training consumptions to have a normal distribution. This makes it easier for the model to learn. Take note of the mean and standard deviation to reverse this operation later.

```
// Compute the scale of the training portion.
let scalerEstimator = ColumnSelector(
    .include(columnNames: ["Temp"]),
    estimator: OptionalUnwrapper().appending(StandardScaler())
)
let trainingDataFrame = DataFrame(dataFrame[trainingPortion])
let scaler = try await scalerEstimator.fitted(to: trainingDataFrame)

// Scale the features.
let scaledDataFrame = try await scaler.applied(to: dataFrame)
let mean = scaler.transformers["Temp"]!.outer.mean
let stddev = scaler.transformers["Temp"]!.outer.standardDeviation
```

Extract features from the dates by using `DateFeatureExtractor`. The extractor creates values in the range `-0.5 ... 0.5` and represents the components you select. Concatenate all features into a single column of `MLShapedArray` values and create a features data frame.

```
// Extract the date features.
let dateFeatureExtractor = ColumnSelector(
    .include(columnNames: ["Date"]),
    transformer: OptionalUnwrapper().appending(
        DateFeatureExtractor(features: [.hour, .weekday, .day, .dayOfYear])
    )
)
// Concatenate the features.
let concatenator = ColumnConcatenator(
    columnSelection: .all,
    concatenatedColumnName: "Features"
)
let preprocessor = try await dateFeatureExtractor.appending(concatenator).fitted(to: scaledDataFrame)
let featuresDataFrame = try await preprocessor.applied(to: dataFrame)
```

Finally, extract features and annotations, and divide the data into training, validation, and testing sets:

```
let features = featuresDataFrame["Features", MLShapedArray.self]
    .filled(with: MLShapedArray())
let annotations = scaledDataFrame["Temp", Float.self]
    .filled(with: 0.0)
    .map({ MLShapedArray(scalars: [Float($0)], shape: [1]) })

// Create the training, validation, and testing splits.
let dayInHours = 24
let monthInHours = 30 * dayInHours
let yearInHours = 12 * monthInHours

let trainingPortion = 0 ..

### Build and train a time-series forecaster

After preparing your training data, you can create a forecaster. The forecaster configuration takes the input window size and forecast window size. Depending on your task you may want to adjust these values. A larger input window provides more context to the model, but results in a larger model. For this example, set the input window size to 14 days (336 samples) and the forecast window size to 4 days (96 samples).

```
var configuration = LinearTimeSeriesForecasterConfiguration(
    inputWindowSize: 14 * dayInHours,
    forecastWindowSize: 4 * dayInHours
)
configuration.maximumIterationCount = 20

let estimator = LinearTimeSeriesForecaster(configuration: configuration)
let model = try await estimator.fitted(to: training, validateOn: validation) { event in
    if let validationLoss = event.metrics[MetricsKey.validationLoss] as? Double {
        print("Validation loss: \(validationLoss)")
    }
}
```

### Evaluate the model

Use your testing set to evaluate your model. Two useful metrics you use to check a forecaster model are the mean-squared error (MSE) and the mean-absolute error (MAE).

```
var mseValues = [Double]()
var maeValues = [Double]()
let predictions = try await model.applied(to: testing.map(\.feature))
let groundTruths = testing.dropFirst(configuration.forecastWindowSize).map(\.annotation)
for (prediction, groundTruth) in zip(predictions, groundTruths) {
    let mse = meanSquaredError(prediction.scalars, groundTruth.scalars)
    let mae = meanAbsoluteError(prediction.scalars, groundTruth.scalars)
    mseValues.append(Double(mse))
    maeValues.append(Double(mae))
}

let mseSum = mseValues.reduce(0, +)
let mse = mseSum / Double(mseValues.count)
print("MSE: \(mse)")

let maeSum = maeValues.reduce(0, +)
let mae = maeSum / Double(maeValues.count)
print("MAE: \(mae)")
```

### Export the model

When you’re satisfied with the model’s accuracy, export it as a Core ML package:

```
try model.export(to: URL(filePath: "forecaster.mlpackage"))
```

Deploy the model you export and use Core ML to perform predictions. When you use the model, you need to concatenate the input window samples into a single shaped array. If you provide more than one window of input, the model returns multiple results in a shaped array.

```
let mlmodel = try MLModel(contentsOf: modelURL)
let testFeatures = MLShapedArray(
    concatenating: testing[0 ..

The model output provides scaled temperatures, so use the mean and standard deviation values to compute the temperatures:

```
let temperatures = result.scalars.map({ $0 * stddev + mean })
print(temperatures)
```

## See Also

### Time-based components

Creating a time-series classifier

Train a machine learning model to predict the class label of time-series signals.

struct DateFeatures

A set of date and time features.

struct DateFeatureExtractor

A time and date feature extractor.

struct LinearTimeSeriesForecaster

A time-series forecasting estimator.

struct LinearTimeSeriesForecasterConfiguration

The configuration for a linear time-series forecaster.

struct TimeSeriesForecasterBatches

A sequence of forecaster batches on a time series shaped array.

struct TimeSeriesForecasterAnnotatedWindows

A sequence of forecasting windows on a time series shaped array.

struct TemporalFeature

A temporal feature contains a segment identifier and a feature value.

protocol TemporalSequence

Async sequence for temporal features.

struct TemporalSegmentIdentifier

Uniquely identifiers a segment of a temporal sequence.

struct SlidingWindows

A sequence of windows on a time series shaped array.

struct SlidingWindowTransformer

A temporal transformer that groups input elements.

struct Downsampler

A temporal transformer that down samples the input stream.

struct VideoReader

A video file reader.

struct TemporalFileSegment

A URL and a time range identifying a specific segment of a time-based (temporal) file.

