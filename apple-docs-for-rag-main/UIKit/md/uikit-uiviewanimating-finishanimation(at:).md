

- UIKit
- UIViewAnimating
-  finishAnimation(at:) 

Instance Method

# finishAnimation(at:)

Finishes the animations and returns the animator to the inactive state.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func finishAnimation(at finalPosition: UIViewAnimatingPosition)
```

**Required**

## Parameters 

`finalPosition`  

The final position for any view properties. Specify UIViewAnimatingPosition.current to leave the view properties unchanged from their current values.

## Discussion

After putting the animator object into the UIViewAnimatingState.stopped state, call this method to perform any final cleanup tasks. It is a programmer error to call this method at any time except after a call to the stopAnimation(_:) method where you pass false for the `withoutFinishing` parameter. Calling this method is not required, but is recommended in cases where you want to ensure that completion blocks or other final tasks are performed.

Implementations of this method are responsible for setting the state of the animator object to UIViewAnimatingState.inactive and for performing any final cleanup tasks, such as executing completion blocks.

## See Also

### Starting and stopping the animations

func startAnimation()

Starts the animation from its current position.

**Required**

func startAnimation(afterDelay: TimeInterval)

Starts the animation after the specified delay.

**Required**

func pauseAnimation()

Pauses a running animation at its current position.

**Required**

func stopAnimation(Bool)

Stops the animations at their current positions.

**Required**

