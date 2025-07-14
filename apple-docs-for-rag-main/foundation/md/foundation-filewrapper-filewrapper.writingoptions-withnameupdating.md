

- Foundation
- FileWrapper
- FileWrapper.WritingOptions
-  withNameUpdating 

Type Property

# withNameUpdating

Whether descendant file wrappers’filename properties are set if the writing succeeds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var withNameUpdating: FileWrapper.WritingOptions { get }
```

## Discussion

This option is necessary when your application passes a URL in the `originalContentsURL` parameter to the write(to:options:originalContentsURL:) method. Without using this option (and reusing child file wrappers properly), subsequent invocations of write(to:options:originalContentsURL:) would not be able to reliably create hard links in a new file package, because the record of names in the old file package would be out of date.

## See Also

### Constants

static var atomic: FileWrapper.WritingOptions

Whether writing is done atomically.

static var atomic: FileWrapper.WritingOptions

Whether writing is done atomically.

