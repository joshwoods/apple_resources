

- Network Extension
-  NEFilterSettings 

Class

# NEFilterSettings

The rules and other settings that define the operation of a filter.

macOS 10.15+

``` source
class NEFilterSettings
```

## Overview

NEFilterDataProvider instances use NEFilterSettings to communicate the desired settings for the filter to the framework. The framework takes care of applying the contained settings to the system.

## Topics

### Creating Filter Settings

init(rules: [NEFilterRule], defaultAction: NEFilterAction)

Creates a new settings instance from an array of rules and a default action.

class NEFilterRule

A rule for filters that combines a rule to match network traffic and an action to take when the rule matches.

### Inspecting Filter Settings

var rules: [NEFilterRule]

An ordered list of rules that define the filter’s operation.

var defaultAction: NEFilterAction

The default action to take for flows of network data that don’t match any of the specified rules.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Changing filter settings

func apply(NEFilterSettings?, completionHandler: ((any Error)?) -> Void)

Applies a set of filtering rules associated with the provider and changes the default filtering action.

