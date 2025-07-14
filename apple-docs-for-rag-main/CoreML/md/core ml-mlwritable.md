

- Core ML
-  MLWritable 

Protocol

# MLWritable

A set of methods that saves a machine learning type to the file system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
protocol MLWritable : NSObjectProtocol
```

## Overview

You use MLWritable to save any MLModel instance that adopts the protocol to the file system.

## Topics

### Saving to a File

func write(to: URL) throws

Exports a machine learning file to the file system.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Saving an Updated Model

var model: any MLModel &amp; MLWritable

The underlying Core ML model stored in memory.

