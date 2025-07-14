

- UIKit
- NSTextElementProvider
-  enumerateTextElements(from:options:using:) 

Instance Method

# enumerateTextElements(from:options:using:)

Enumerates text elements starting at the text location you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func enumerateTextElements(
    from textLocation: (any NSTextLocation)?,
    options: NSTextContentManager.EnumerationOptions = [],
    using block: (NSTextElement) -> Bool
) -> (any NSTextLocation)?
```

**Required**

## Parameters 

`textLocation`  

The NSTextLocation at which to start the enumeration.

`options`  

One of the possible `NSTextElementProviderEnumerationOptions` directions.

`block`  

A block you use to evaluate whether to continue the enumeration or tell the method to stop. Return `false` to end the enumeration process.

## Return Value

An `NSTextLocation`.

## Discussion

If `textLocation` is `nil`, the method uses `documentRange.location` for forward enumeration and `documentRange.endLocation` for reverse enumeration. When enumerating backward, the method starts with the element preceding the one containing `textLocation`. If enumerated at least one element, it returns the edge of the enumerated range.

The enumerated range might not match the range of the last element returned. It enumerates the elements in the sequence, but it can skip a range (it can limit the maximum number of text elements enumerated for a single invocation or hide some elements from the layout).

Returning `NO` or `false` from block breaks out of the enumeration.

## See Also

### Accessing and updating the text

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location from location with offset you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement]?)

Replaces the characters specified by range with the text elements you provide.

**Required**

