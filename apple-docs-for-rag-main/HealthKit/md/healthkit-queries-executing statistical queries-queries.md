

- HealthKit
- Queries
-  Executing Statistical Queries 

Article

# Executing Statistical Queries

Create and run statistical queries.

## Overview

Statistical queries calculate common statistics over a matching set of samples, for example by returning the minimum value, the maximum value, or the sum of all the values.

### Create the Object Type and Predicate

Start by creating the type object for the desired samples. The following example creates a type object for energy consumed.

```
guard let energyConsumed = HKSampleType.quantityType(forIdentifier: HKQuantityTypeIdentifier.dietaryEnergyConsumed) else {
    // This should never fail when using a defined constant.
    fatalError("*** Unable to get the step count type ***")
}
```

Next, create a predicate for samples created between midnight last night and midnight tonight.

```
let calendar = NSCalendar.current
let now = Date()
let components = calendar.dateComponents([.year, .month, .day], from: now)

guard let startDate = calendar.date(from: components) else {
    fatalError("*** Unable to create the start date ***")
}

guard let endDate = calendar.date(byAdding: .day, value: 1, to: startDate) else {
    fatalError("*** Unable to create the end date ***")
}

let today = HKQuery.predicateForSamples(withStart: startDate, end: endDate, options: [])
```

You use these values to create the query.

### Create the Query

To create the statistical query, call the init(quantityType:quantitySamplePredicate:options:completionHandler:) initializer. The following code creates a statistical query that calculates the total energy consumed during the specified time period.

```
let query = HKStatisticsQuery(quantityType: energyConsumed, quantitySamplePredicate: today, options: .cumulativeSum) { (query, statisticsOrNil, errorOrNil) in

    guard let statistics = statisticsOrNil else {
        // Handle any errors here.
        return
    }

    let sum = statistics.sumQuantity()
    let totalCaloriesConsumed = sum?.doubleValue(for: HKUnit.largeCalorie())

    // Update your app here.

    // The results come back on an anonymous background queue.
    // Dispatch to the main queue before modifying the UI.

    DispatchQueue.main.async {
        // Update the UI here.
    }
}
```

The query returns a statistics object that contains the values calculated by the query. The callback handler should check for errors before accessing the statistics. It should also dispatch updates to the user interface back to the main thread.

### Run the Query

After the query is instantiated, you run it by calling the HealthKit store’s execute(_:) method on the HealthKit store.

```
store.execute(query)
```

This method runs the query on an anonymous background queue. When the query is complete, it executes the results handler on the same background queue (but not necessarily on the same thread).

## See Also

### Statistics

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

struct HKStatisticsQueryDescriptor

A query descriptor that calculates the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

struct HKStatisticsCollectionQueryDescriptor

A query descriptor that gathers a collection of statistics calculated over a series of fixed-length time intervals.

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

