

- Foundation
-  ProgressReporting 

Protocol

# ProgressReporting

An interface for objects that report progress using a single progress instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ProgressReporting : NSObjectProtocol
```

## Overview

Create the returned progress object using ProgressReporting. The resulting object has no parent allowing the caller to add it to a progress tree using ProgressReporting.

You can return a single progress object or a progress tree. If you are creating a progress tree, add the children to the returned progress object as described in Reporting Progress for Multiple Operations.

You are responsible for setting and updating the ProgressReporting of any Progress object you create.

## Topics

### Custom Class Progress

var progress: Progress

The progress object returned by the class.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSBundleResourceRequest
- OperationQueue
- URLSessionDataTask
- URLSessionDownloadTask
- URLSessionStreamTask
- URLSessionTask
- URLSessionUploadTask
- URLSessionWebSocketTask

## See Also

### Progress

class Progress

An object that conveys ongoing progress to the user for a specified task.

