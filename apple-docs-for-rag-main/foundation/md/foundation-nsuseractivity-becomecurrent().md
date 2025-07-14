

- Foundation
- NSUserActivity
-  becomeCurrent() 

Instance Method

# becomeCurrent()

Marks the activity as currently in use by the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func becomeCurrent()
```

## Mentioned in 

Creating a user activity object

## Discussion

Call this method to let the system know that the user is performing the associated activity. The system makes this object the current user activity object, which makes it available for Handoff and search indexing. If another user activity object was previously active, that object is made inactive.

Don’t call this method when providing a user activity object for a Siri request. Siri holds on to user activity objects and passes them along to your app automatically in response to specific events.

If you previously called the invalidate() method on the current object, calling this method has no effect.

## See Also

### Registering and invalidating user activities

func resignCurrent()

Marks this activity object as inactive without invalidating it.

func invalidate()

Invalidates an activity and marks it as no longer eligible for continuation.

