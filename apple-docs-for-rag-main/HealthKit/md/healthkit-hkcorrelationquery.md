

- HealthKit
-  HKCorrelationQuery 

Class

# HKCorrelationQuery

A query that performs complex searches based on the correlation’s contents, and returns a snapshot of all matching samples.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCorrelationQuery
```

## Mentioned in 

Reading data from HealthKit

## Overview

Correlation samples act as a container, grouping multiple quantity or category samples. While you can use HKSample objects to search for correlations, correlation queries allow more complex filtering based on the contained samples. Specifically, correlation queries let you provide a separate predicate for each of the sample types stored in the correlation. A correlation is returned only if the correlation’s predicate and all of the sample predicates match.

### Requesting Permission to Share and Read

Unlike other sample types, you do not request permission to share and read correlation types directly. Instead, you request permission to share and read each of the sample types contained within the correlation.

When saving a correlation, the app must have permission to share all of the contained objects. If the app does not have permission to share one or more of the contained objects, the operation fails.

When your app queries for correlation data, HealthKit only returns samples that contain objects you have permission to read. If the app has permission to read only some of the contained objects, HealthKit still returns the correlation; however, the correlation appears to only contain those objects that your app has permission to read. HealthKit hides all of the other contained objects from your app.

### Executing Queries

You create a correlation query by calling the init(type:predicate:samplePredicates:completion:) initializer. After the query is instantiated, you run it by calling the HealthKit store’s execute(_:) method. This method runs the query on an anonymous background queue. When the query is complete, it executes the results handler on the same background queue (though not necessarily the same thread). Typically, you dispatch these results back to the main thread to update your user interface.

The following example builds a correlation query that searches for food samples with more than 800 calories.

- Swift
- Objective-C

```
var highCalorieFoods: [HKCorrelationQuery] = []

let highCalorie = HKQuantity(unit: HKUnit.kilocalorieUnit(),
                             doubleValue: 800.0);

let greaterThanHighCalorie = HKQuery.predicateForQuantitySamplesWithOperatorType(
    .GreaterThanOrEqualToPredicateOperatorType, quantity: highCalorie)

let energyConsumed = HKObjectType.quantityTypeForIdentifier(
    HKQuantityTypeIdentifierDietaryEnergyConsumed)

let samplePredicates = [energyConsumed: greaterThanHighCalorie]

let foodType = HKCorrelationType.correlationTypeForIdentifier(
    HKCorrelationTypeIdentifierFood)

let query = HKCorrelationQuery(type: foodType, predicate: nil, samplePredicates: samplePredicates)
{
    query, results, error in

    if let correlations = results as? [HKCorrelationQuery] {
        for correlation in correlations {
            highCalorieFoods.append(correlation)
        }
    }
    else {
        // Provide proper error handling here...
        println("An error occurred while searching for high calorie food: \(error.localizedDescription)")
        abort()
    }

    println("Found \(highCalorieFoods.count) foods: \(highCalorieFoods)")
}

healthStore.executeQuery(query)
```

```
```

It begins by setting up an array to store our high calorie foods. Next, the sample code creates a predicate that matches quantities greater than or equal to 800 kcal. It then creates a dictionary using a quantity type object for dietary energy consumed as the key and the newly-created predicate as the value. It uses this dictionary as the sample predicates for a correlation query.

In the query’s completion handler, the sample code first checks to see if an error occurred. If no errors occurred, it adds the results to the array of high calorie foods. Then it logs the number of matching samples found, and the contents of the high calorie foods array.

Once the sample code finishes declaring the completion handler, the query is ready to use. The sample code simply executes the query on the HeathKit store.

### Subclassing Correlation Queries

Like many HealthKit classes, the `HKCorrelationQuery` class should not be subclassed.

## Topics

### Creating Correlation Queries

init(type: HKCorrelationType, predicate: NSPredicate?, samplePredicates: [HKSampleType : NSPredicate]?, completion: (HKCorrelationQuery, [HKCorrelation]?, (any Error)?) -> Void)

Instantiates and returns a correlation query.

### Getting Property Data

var correlationType: HKCorrelationType

The type of correlation to search for.

var samplePredicates: [HKSampleType : NSPredicate]?

A dictionary whose keys are HKSampleType instances and whose values are NSPredicate instances.

## Relationships

### Inherits From

- HKQuery

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Basic queries

struct HKSampleQueryDescriptor

A query interface that reads samples using Swift concurrency.

class HKSampleQuery

A general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

class HKQueryDescriptor

A descriptor that specifies a set of samples based on the data type and a predicate.

class HKQuery

An abstract class for all the query classes in HealthKit.

