

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  addPasses(\_:withCompletionHandler:) 

Instance Method

# addPasses(\_:withCompletionHandler:)

Presents a user interface for adding multiple passes at once.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func addPasses(
    _ passes: [PKPass],
    withCompletionHandler completion: ((PKPassLibraryAddPassesStatus) -> Void)? = nil
)
```

``` source
func addPasses(_ passes: [PKPass]) async -> PKPassLibraryAddPassesStatus
```

## Parameters 

`passes`  

The passes to add.

`completion`  

The completion handler that PassKit calls after the user selects an action. This handler takes the following parameter:

`status`  
A PKPassLibraryAddPassesStatus value that indicates whether PassKit adds the passes. If the user selects to review the passes, PassKit sets the status to PKPassLibraryAddPassesStatus.shouldReviewPasses. In this case, you must present an instance of PKAddPassesViewController to let the user review and add the passes.

## Discussion

Use this method whenever the user initiates an action that generates a single pass (like purchasing a concert ticket) or multiple passes (like checking into a multiconnection flight). The user receives a prompt to confirm the overall action or to review the passes individually. If you want to force the user to review individual passes visually before adding them, use an instance of PKAddPassesViewController.

## See Also

### Adding passes

func canAddSecureElementPass(primaryAccountIdentifier: String) -> Bool

Returns a Boolean value that indicates whether PassKit can add a Secure Element pass for the specified account.

func canAddFelicaPass() -> Bool

Returns a Boolean value that indicates whether the library can add FeliCa™ passes.

enum PKPassLibraryAddPassesStatus

Statuses that PassKit uses when it adds passes to the pass library.

