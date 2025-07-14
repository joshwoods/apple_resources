

- BrowserEngineKit
- BEScrollView
-  delegate 

Instance Property

# delegate

The delegate of the scroll view.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
weak var delegate: (any BEScrollViewDelegate)? { get set }
```

## Overview

The `BEScrollView` class doesn’t retain the delegate, which must conform to the BEScrollViewDelegate protocol.

