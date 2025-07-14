

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:requestsRangeInContextWithIdentifierFor:completion:) Deprecated

Instance Method

# writingToolsCoordinator(\_:requestsRangeInContextWithIdentifierFor:completion:)

Asks the delegate to provide the location of the character at the specified point in your view’s coordinate system.

iOS 18.2–18.4DeprecatediPadOS 18.2–18.4DeprecatedMac Catalyst 18.2–18.4Deprecated

``` source
optional func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    requestsRangeInContextWithIdentifierFor point: CGPoint,
    completion: @escaping (NSRange, UUID) -> Void
)
```

``` source
optional func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    rangeInContextWithIdentifierFor point: CGPoint
) async -> (NSRange, UUID)
```

Deprecated

In iOS 18.4 and later and visionOS 2.4 and later, UIWritingToolsCoordinator automatically determines the location of the character at the specified point in your view's coordinate system and no longer calls this method.

## Parameters 

`writingToolsCoordinator`  

The coordinator object requesting information from your custom view.

`point`  

A point in your view’s coordinate space. Find the location of the text under this point, if any.

`completion`  

A handler to execute with the required information. This handler has no return value and takes an NSRange and UUID as parameters. Set the range to the character’s location in one of your UIWritingToolsCoordinator.Context objects, which you specify using the UUID parameter. You must call this handler at some point during your method’s implementation.

## Discussion

When someone interacts with your view during a proofreading operation, Writing Tools calls this method to get the location of the interaction. If the interaction occurs in the text of one of your UIWritingToolsCoordinator.Context objects, configure an NSRange with the character’s location in that context object and a length of `1`. If the interaction occurs outside of the text of your context objects, configure the range with a location of `NSNotFound`.

When specifying the location of a character in your context object, provide a location relative to the start of your context object’s text. The first character in a context object’s text is always at location `0`, and it’s your responsibility to track the location of the context object’s text in your text storage object. When the context object’s text begins in the middle of your text storage, subtract the starting location of the context object’s text from the location you specify in your range value. For example, if the context object’s text starts at character `100` in your text storage, and an interaction occurs with the character at location `102`, specify a range with a location of `2` and a length of `1`.

## See Also

### Displaying proofreading marks

func writingToolsCoordinator(UIWritingToolsCoordinator, requestsBoundingBezierPathsFor: NSRange, in: UIWritingToolsCoordinator.Context, completion: ([UIBezierPath]) -> Void)

Asks the delegate to provide the bounding paths for the specified text in your view.

**Required**

func writingToolsCoordinator(UIWritingToolsCoordinator, requestsUnderlinePathsFor: NSRange, in: UIWritingToolsCoordinator.Context, completion: ([UIBezierPath]) -> Void)

Asks the delegate to provide an underline shape for the specified text during a proofreading session.

**Required**

