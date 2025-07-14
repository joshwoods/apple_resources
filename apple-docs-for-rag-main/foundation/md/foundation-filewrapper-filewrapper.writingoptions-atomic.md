

- Foundation
- FileWrapper
- FileWrapper.WritingOptions
-  atomic 

Type Property

# atomic

Whether writing is done atomically.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var atomic: FileWrapper.WritingOptions { get }
```

## Discussion

You can use this option to ensure that, when overwriting a file package, the overwriting either completely succeeds or completely fails, with no possibility of leaving the file package in an inconsistent state. Because this option causes additional I/O, you shouldn’t use it unnecessarily. For example, don’t use this option in an override of `-[NSDocument` write(to:ofType:)`]`, because `NSDocument` safe-saving is already done atomically.

## See Also

### Constants

static var withNameUpdating: FileWrapper.WritingOptions

Whether descendant file wrappers’filename properties are set if the writing succeeds.

static var withNameUpdating: FileWrapper.WritingOptions

Whether descendant file wrappers’filename properties are set if the writing succeeds.

