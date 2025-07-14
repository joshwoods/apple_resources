

- HealthKit
-  HKSourceQueryDescriptor 

Structure

# HKSourceQueryDescriptor

A query interface that uses Swift concurrency to read the apps and devices that produced the matching samples.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKSourceQueryDescriptor where Sample : HKSample
```

## Mentioned in 

Reading data from HealthKit

## Overview

Use HKSourceQueryDescriptor to run a general query that returns a snapshot of all the apps and devices that have saved matching data to the HealthKit store.

```
// Create the source descriptor.
let sourceDescriptor = HKSourceQueryDescriptor(predicate: .workout())

// Read the source data from the HealthKit store.
let sources = try await sourceDescriptor.result(for: store)

for source in sources {
    // Process the sources here.
    print(source)
}
```

When you call the descriptor’s result(for:) method, it creates and executes an HKSourceQuery in the background, passing the results as an array of HKSource instances.

## Topics

### Creating Source Query Descriptors

init(predicate: HKSamplePredicate&lt;Sample>)

Creates a source query descriptor.

### Running Queries

func result(for: HKHealthStore) async throws -> [HKSource]

Runs a one-shot query that asynchronously returns a snapshot of all the sources that saved matching data.

### Accessing Query Properties

var predicate: HKSamplePredicate&lt;Sample>

A predicate that limits the data used by the query.

### Default Implementations

HKAsyncQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery

  Conforms when `Sample` inherits `HKSample`.

## See Also

### Sources and devices

class HKSourceRevision

An object indicating the source of a HealthKit sample.

class HKSource

An object indicating the app or device that created a HealthKit sample

class HKDevice

A device that generates data for HealthKit.

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

