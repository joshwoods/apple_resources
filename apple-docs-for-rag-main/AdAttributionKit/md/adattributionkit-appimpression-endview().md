

- AdAttributionKit
- AppImpression
-  endView() 

Instance Method

# endView()

Ends the view-through impression when the ad content corresponding to the impression disappears.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
func endView() async throws
```

## Mentioned in 

Presenting ads in your app

## Discussion

End the view-through impression, as the following example shows:

```
   func handleAdDisappeared(impression: AppImpression) async {
       do {
           try await impression.endView()
       }
       catch {
           print("Failed to end view-through impression: \(error).")
       }
   }    
```

