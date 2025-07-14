

- Network Extension
- NEFilterManager
-  NEFilterManager.Grade 

Enumeration

# NEFilterManager.Grade

A type for the grade or priority of the filter.

macOS 10.15+

``` source
enum Grade
```

## Topics

### Grades

case firewall

A grade for filters that act as firewalls, blocking some network traffic.

case inspector

A grade for filters that act as inspectors of network traffic.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Prioritizing filters

var grade: NEFilterManager.Grade

The grade of the filter, which determines when it acts relative to other filters.

