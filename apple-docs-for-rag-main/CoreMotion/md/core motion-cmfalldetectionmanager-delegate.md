

- Core Motion
- CMFallDetectionManager
-  delegate 

Instance Property

# delegate

A delegate that can receive notifications about fall detection events.

watchOS 7.2+

``` source
weak var delegate: (any CMFallDetectionDelegate)? { get set }
```

## See Also

### Handling Events

protocol CMFallDetectionDelegate

A delegate that receives information about fall detection events and authorization status changes.

