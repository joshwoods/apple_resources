

- UIKit
- UIStoryboardSegue
-  identifier 

Instance Property

# identifier

The identifier for the segue object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var identifier: String? { get }
```

## Discussion

You assign identifiers to your segues in Interface Builder. An identifier is a string that your application uses to distinguish one segue from another. For example, if you have a source view controller that can segue to two or more different destination view controllers, you’d assign different identifiers to each segue so that the source view controller’s prepare(for:sender:) method could tell them apart and prepare each segue appropriately.

## See Also

### Accessing the segue attributes

var source: UIViewController

The source view controller for the segue.

var destination: UIViewController

The destination view controller for the segue.

