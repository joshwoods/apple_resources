

- Network Extension
- NEFilterManager
-  grade 

Instance Property

# grade

The grade of the filter, which determines when it acts relative to other filters.

macOS 10.15+

``` source
var grade: NEFilterManager.Grade { get set }
```

## Discussion

The default grade is NEFilterManager.Grade.firewall.

## See Also

### Prioritizing filters

enum Grade

A type for the grade or priority of the filter.

