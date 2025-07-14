

- Foundation
- NSBackgroundActivityScheduler
-  invalidate() 

Instance Method

# invalidate()

Prevents the background activity from being scheduled again.

macOS 10.10+

``` source
func invalidate()
```

## Discussion

When `invalidate` is used to stop an activity that is currently executing, the activity will still finish executing.

See Stop Activity.

