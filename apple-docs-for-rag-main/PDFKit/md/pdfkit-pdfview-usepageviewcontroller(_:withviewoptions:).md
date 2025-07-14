

- PDFKit
- PDFView
-  usePageViewController(\_:withViewOptions:) 

Instance Method

# usePageViewController(\_:withViewOptions:)

Changes the scroll view to use a `UIPageViewController` to layout and navigate pages.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func usePageViewController(
    _ enable: Bool,
    withViewOptions viewOptions: [AnyHashable : Any]? = nil
)
```

## See Also

### Displaying as Book

var displaysAsBook: Bool

A Boolean value indicating whether the view will display the first page as a book cover (meaningful only when the document is in two-up or two-up continuous display mode).

var isUsingPageViewController: Bool

A Boolean value indicating whether the scroll view is using a `UIPageViewController`.

