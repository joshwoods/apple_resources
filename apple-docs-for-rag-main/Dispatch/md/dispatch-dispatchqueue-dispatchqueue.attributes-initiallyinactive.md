

- Dispatch
- DispatchQueue
- DispatchQueue.Attributes
-  initiallyInactive 

Type Property

# initiallyInactive

The newly created queue is inactive.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let initiallyInactive: DispatchQueue.Attributes
```

## Discussion

Normally, a newly created queue schedules submitted blocks for execution immediately. Use this attribute to prevent the queue from scheduling blocks until you call its activate() method.

## See Also

### Attributes

static let concurrent: DispatchQueue.Attributes

The queue schedules tasks concurrently.

