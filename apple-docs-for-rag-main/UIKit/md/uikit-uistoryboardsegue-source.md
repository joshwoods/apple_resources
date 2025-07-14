

- UIKit
- UIStoryboardSegue
-  source 

Instance Property

# source

The source view controller for the segue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var source: UIViewController { get }
```

## Discussion

This property contains the view controller whose contents are displayed at the beginning of the segue.

## See Also

### Accessing the segue attributes

var destination: UIViewController

The destination view controller for the segue.

var identifier: String?

The identifier for the segue object.

