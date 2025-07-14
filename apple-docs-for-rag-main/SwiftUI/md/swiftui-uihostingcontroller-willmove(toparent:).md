

- SwiftUI
- UIHostingController
-  willMove(toParent:) 

Instance Method

# willMove(toParent:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
override dynamic func willMove(toParent parent: UIViewController?)
```

## See Also

### Responding to view-related events

func loadView()

func viewWillAppear(Bool)

Notifies the view controller that its view is about to be added to a view hierarchy.

func viewDidAppear(Bool)

Notifies the view controller that its view has been added to a view hierarchy.

func viewWillDisappear(Bool)

Notifies the view controller that its view will be removed from a view hierarchy.

func viewDidDisappear(Bool)

func didMove(toParent: UIViewController?)

func viewWillTransition(to: CGSize, with: any UIViewControllerTransitionCoordinator)

func viewWillLayoutSubviews()

func target(forAction: Selector, withSender: Any?) -> Any?

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this view controller.

