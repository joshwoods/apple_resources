

- UIKit
- UIFindInteractionDelegate
-  findInteraction(\_:sessionFor:) 

Instance Method

# findInteraction(\_:sessionFor:)

Provides the object for managing the state, presentation, and behavior of the search.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func findInteraction(
    _ interaction: UIFindInteraction,
    sessionFor view: UIView
) -> UIFindSession?
```

**Required**

## Parameters 

`interaction`  

The interaction object triggering the find panel.

`view`  

The view you provide a find session object for.

## Return Value

Returns an object the find interaction uses to manage the state, presentation, and behavior of the search. To prevent the find panel from appearing, return `nil`.

## Discussion

Implement the UITextSearching protocol on the class that encapsulates the searchable content for your view to use an instance of UITextSearchingFindSession as the session object. Alternatively, you can subclass UIFindSession to manage the details of the session using a custom class.

