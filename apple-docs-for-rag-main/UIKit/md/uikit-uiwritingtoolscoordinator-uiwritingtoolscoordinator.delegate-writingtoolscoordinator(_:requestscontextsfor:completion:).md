

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:requestsContextsFor:completion:) 

Instance Method

# writingToolsCoordinator(\_:requestsContextsFor:completion:)

Asks your delegate to provide the text to evaluate during the Writing Tools operation.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    requestsContextsFor scope: UIWritingToolsCoordinator.ContextScope,
    completion: @escaping ([UIWritingToolsCoordinator.Context]) -> Void
)
```

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    contextsFor scope: UIWritingToolsCoordinator.ContextScope
) async -> [UIWritingToolsCoordinator.Context]
```

**Required**

## Parameters 

`writingToolsCoordinator`  

The coordinator object requesting information from your custom view.

`scope`  

The amount of text the coordinator requested. Use this property to determine if Writing Tools is evaluating all of your text or only a subset.

`completion`  

A completion block to execute with the required information. You must execute this block once at end of your method’s implementation. The block has no return value and takes an array of UIWritingToolsCoordinator.Context objects that contain the requested information.

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

At the start of every operation, the UIWritingToolsCoordinator object calls this method to request the text to evaluate. Use this method to create one or more UIWritingToolsCoordinator.Context objects with your view’s text. Create only one UIWritingToolsCoordinator.Context object if your view has only one text storage object. If your view contains multiple text storage objects, create separate UIWritingToolsCoordinator.Context objects for each text storage object. Writing Tools returns updates for each context object separately, making it easier for you to incorporate changes into the correct text storage object. Don’t create multiple context objects if your view has only one text storage object.

The `scope` parameter tells you what content Writing Tools expects you to provide in your context object. For example, Writing Tools expects you to provide the selected text when the parameter contains the UIWritingToolsCoordinator.ContextScope.userSelection option. When Writing Tools requests a subset of your overall text, include some of the surrounding text in your context object too. Writing Tools can use the extra text you provide to improve the results of its evaluation. For example, it might use an entire paragraph, instead of only the selected sentence, to evaluate ways to rewrite that sentence. It’s best to include the text up to the nearest paragraph boundary before and after the selection. If you include extra text in your context object, set the range property to the range of the selected text.

Note

When a context object stores only a subset of your view’s text, record additional information to map the location of that text to the correct location in your view’s text storage. Keep that information up-to-date throughout the Writing Tools session.

Pass the context objects you create to the provided completion handler before your method returns. Writing Tools waits for you to call the completion handler before proceeding with the operation.

