

- Swift
-  Job 

Structure

# Job

Deprecated equivalent of ExecutorJob.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+visionOS 1.0+

``` source
@frozen
struct Job
```

## Overview

A unit of schedulable work.

Unless you’re implementing a scheduler, you don’t generally interact with jobs directly.

## Topics

### Initializers

init(UnownedJob)Deprecated

init(ExecutorJob)Deprecated

### Instance Properties

var description: StringDeprecated

var priority: JobPriorityDeprecated

### Instance Methods

func runSynchronously(on: UnownedSerialExecutor)

Run this job on the passed in executor.

## Relationships

### Conforms To

- Sendable

