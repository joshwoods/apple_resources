

- BrowserEngineKit
- BEScrollViewDelegate
-  parentScrollView(for:) 

Instance Method

# parentScrollView(for:)

Indicates that a sibling scroll view in the view hierarchy acts as the scroll view’s container in the Document Object Model (DOM).

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
optional func parentScrollView(for scrollView: BEScrollView) -> BEScrollView?
```

## Parameters 

`scrollView`  

The scroll view to return the logically containing scroll view for.

## Return Value

The scroll view that is logically the container of the provided scroll view. Return `nil` to get the default behavior of recursively searching the scroll view’s superview hierarchy for a containing scroll view.

## Overview

To correctly render some websites, you might need to create BEScrollView objects that are siblings in the view hierarchy, but nested in the DOM. In these situations, implement `parentScrollView(for:)` in the delegate for the scroll view that is logically the contained scroll view in the DOM, and return the logically containing scroll view. The containing scroll view needs to be visually beneath the contained scroll view.

