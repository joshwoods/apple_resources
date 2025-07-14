

- PDFKit
- PDFView
-  isUsingPageViewController 

Instance Property

# isUsingPageViewController

A Boolean value indicating whether the scroll view is using a `UIPageViewController`.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var isUsingPageViewController: Bool { get }
```

## See Also

### Displaying as Book

var displaysAsBook: Bool

A Boolean value indicating whether the view will display the first page as a book cover (meaningful only when the document is in two-up or two-up continuous display mode).

func usePageViewController(Bool, withViewOptions: [AnyHashable : Any]?)

Changes the scroll view to use a `UIPageViewController` to layout and navigate pages.

