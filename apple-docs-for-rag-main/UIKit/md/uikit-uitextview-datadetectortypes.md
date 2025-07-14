

- UIKit
- UITextView
-  dataDetectorTypes 

Instance Property

# dataDetectorTypes

The types of data that convert to tappable URLs in the text view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dataDetectorTypes: UIDataDetectorTypes { get set }
```

## Discussion

You can use this property to specify the types of data (phone numbers, `http` links, and so on) that should be automatically converted to URLs in the text view. When tapped, the text view opens the application responsible for handling the URL type and passes it the URL. Note that data detection does not occur if the text view’s isEditable property is set to true.

## See Also

### Formatting special data in text

struct UIDataDetectorTypes

Constants that define the types of information to detect in text-based content.

