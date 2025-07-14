

- UIKit
- UITextFormattingViewController
-  UITextFormattingViewController.FormattingDescriptor 

Structure

# UITextFormattingViewController.FormattingDescriptor

iOS 18.0+iPadOS 18.0+

``` source
struct FormattingDescriptor
```

## Topics

### Initializers

init()

init(attributes: [NSAttributedString.Key : Any])

init(attributes: AttributeContainer)

init(string: some AttributedStringProtocol)

init(string: NSAttributedString, range: NSRange)

### Instance Properties

var fonts: [UIFont]

var formattingStyleKey: String?

var highlights: Set&lt;UITextFormattingViewController.Highlight>

var lineHeight: Double?

var strikethroughPresent: Bool

var textAlignments: Set&lt;UITextFormattingViewController.TextAlignment>

var textColors: [UIColor]

var textLists: Set&lt;UITextFormattingViewController.TextList>

var underlinePresent: Bool

