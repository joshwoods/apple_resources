

- UIKit
- UIViewController
-  updateViewConstraints() 

Instance Method

# updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func updateViewConstraints()
```

## Discussion

Override this method to optimize changes to your constraints.

Note

It is almost always cleaner and easier to update a constraint immediately after the affecting change has occurred. For example, if you want to change a constraint in response to a button tap, make that change directly in the button’s action method.

You should only override this method when changing constraints in place is too slow, or when a view is producing a number of redundant changes.

To schedule a change, call setNeedsUpdateConstraints() on the view. The system then calls your implementation of updateViewConstraints() before the layout occurs. This lets you verify that all necessary constraints for your content are in place at a time when your properties are not changing.

Your implementation must be as efficient as possible. Do not deactivate all your constraints, then reactivate the ones you need. Instead, your app must have some way of tracking your constraints, and validating them during each update pass. Only change items that need to be changed. During each update pass, you must ensure that you have the appropriate constraints for the app’s current state.

Do not call setNeedsUpdateConstraints() inside your implementation. Calling setNeedsUpdateConstraints() schedules another update pass, creating a feedback loop.

Important

Call `[super updateViewConstraints]` as the final step in your implementation.

In iOS 18 and later, UIKit supports automatic trait tracking inside this method for traits from this view controller’s `traitCollection` and the `traitCollection` of its view. For more information, see Automatic trait tracking.

## See Also

### View controllers

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

