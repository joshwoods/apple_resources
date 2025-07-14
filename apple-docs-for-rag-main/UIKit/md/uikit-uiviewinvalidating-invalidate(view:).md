

- UIKit
- UIViewInvalidating
-  invalidate(view:) 

Instance Method

# invalidate(view:)

Indicates to the system that an aspect of a view is invalid and triggers the necessary update.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOSSwift 5.1+

``` source
func invalidate(view: UIView)
```

**Required**

## Parameters 

`view`  

The view that requires invalidating.

## Discussion

A type that conforms to UIViewInvalidating implements this method to perform any actions necessary to notify the system that an aspect of your view is invalid. For more info, see UIView.Invalidating.

## See Also

### Invalidating the view

enum Invalidations

Changes that cause an aspect of a view to be invalid and require an update.

