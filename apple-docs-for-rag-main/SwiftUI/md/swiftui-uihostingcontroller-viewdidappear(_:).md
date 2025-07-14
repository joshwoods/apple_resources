

- SwiftUI
- UIHostingController
-  viewDidAppear(\_:) 

Instance Method

# viewDidAppear(\_:)

Notifies the view controller that its view has been added to a view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
override dynamic func viewDidAppear(_ animated: Bool)
```

## Parameters 

`animated`  

If `true`, the view is being added using an animation.

## Discussion

SwiftUI calls this method after adding the hosting controller’s root view to the view hierarchy. You can override this method to perform custom tasks associated with the appearance of the view. If you override this method, you must call `super` at some point in your implementation.

## See Also

### Responding to view-related events

func loadView()

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view will be removed from a view hierarchy.

func viewDidDisappear(Bool)

func willMove(toParent: UIViewController?)

func didMove(toParent: UIViewController?)

func viewWillTransition(to: CGSize, with: any UIViewControllerTransitionCoordinator)

func viewWillLayoutSubviews()

func target(forAction: Selector, withSender: Any?) -> Any?

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this view controller.

