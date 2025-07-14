

- UIKit
-  UIActivityItemProvider 

Class

# UIActivityItemProvider

A proxy for data that passes to an activity view controller.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIActivityItemProvider
```

## Overview

You can use a provider object in situations where you want to make data available for use by an activity but you want to delay providing that data until it’s actually needed. For example, you might use a provider object to represent a large video file that needs to be processed before it can be shared to a user’s social media account.

When you initialize a UIActivityViewController object, you can pass a provider object in addition to any other data objects. When the user selects an activity, the activity view controller adds your provider object (which is also an operation object) to an operation queue so that it can begin to gather or process the needed data.

### Subclassing notes

You must subclass `UIActivityItemProvider` and implement its item method, which is called to generate the item data. You implement this method instead of the normal main() method you’d implement for an operation object. (The main() method calls the item method when the operation object is executed.) Your implementation of the item method should do whatever work is necessary to create and return the data.

## Topics

### Initializing the provider

init(placeholderItem: Any)

Initializes and returns a provider object with the specified placeholder data.

### Accessing the provider attributes

var item: Any

Generates and returns the actual data-bearing object.

var placeholderItem: Any?

The placeholder object you specified at initialization time.

var activityType: UIActivity.ActivityType?

The type of the activity object that is expecting the data.

## Relationships

### Inherits From

- Operation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIActivityItemSource

## See Also

### Services

class UIActivity

An abstract class that you subclass to implement app-specific services.

class UIActivityViewController

A view controller that you use to offer standard services from your app.

protocol UIActivityItemSource

A set of methods that an activity view controller uses to retrieve the data items to act on.

