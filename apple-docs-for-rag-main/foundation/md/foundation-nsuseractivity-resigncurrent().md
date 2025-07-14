

- Foundation
- NSUserActivity
-  resignCurrent() 

Instance Method

# resignCurrent()

Marks this activity object as inactive without invalidating it.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func resignCurrent()
```

## Discussion

Calling this method marks the user activity as no longer current, but doesn’t invalidate it entirely. You can call this method when you want to stop advertising the activity for continuation and search indexing only temporarily. You may call becomeCurrent() later to restore this object as the current activity.

## See Also

### Registering and invalidating user activities

func becomeCurrent()

Marks the activity as currently in use by the user.

func invalidate()

Invalidates an activity and marks it as no longer eligible for continuation.

