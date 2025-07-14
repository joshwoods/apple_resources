

- AppKit
- NSAnimationContext
-  runAnimationGroup(\_:completionHandler:) 

Type Method

# runAnimationGroup(\_:completionHandler:)

Allows you to specify a completion block body after the set of animation actions whose completion will trigger the completion block.

macOS 10.7+

``` source
class func runAnimationGroup(
    _ changes: (NSAnimationContext) -> Void,
    completionHandler: (() -> Void)? = nil
)
```

``` source
class func runAnimationGroup(_ changes: (NSAnimationContext) -> Void) async
```

## Parameters 

`changes`  

A block object containing animations for this transaction group.

The `context` parameter passes the thread’s current `NSAnimationContext` to the Block as a convenience, so code within the Block that wants to change or query properties of the current `context` does not have to call current.

The block object returns no value.

`completionHandler`  

A Block object called when animations for this transaction group are completed.

The Block object takes no parameters and returns no value.

## Discussion

Using this method allows you to more naturally group animations and an completion Block.

An example use is as follows. Using this method you would write the following code fragment:

```
[NSAnimationContext runAnimationGroup:^(NSAnimationContext *context){
    // Start some animations.
    [[myView animator] setFrameSize:newViewSize];
    [[myWindow animator] setFrame:newWindowFrame display:YES];
  } completionHandler:^{
    // This block will be invoked when all of the animations
    // started above have completed or been cancelled.
    NSLog(@"All done!");
}];
```

The above code is semantically equivalent to the following:

```
[NSAnimationContext beginGrouping];
    [NSAnimationContext setCompletionHandler:^{
       // This block will be invoked when all of the animations
       //  started below have completed or been cancelled.
        NSLog(@"All done!");
    }];
    // Start some animations.
    [[myView animator] setFrameSize:newViewSize];
    [[myWindow animator] setFrame:newWindowFrame display:YES];
[NSAnimationContext endGrouping];
```

## See Also

### Animation Completion Handlers

var completionHandler: (() -> Void)?

A completion Block that is called when the animations in the grouping are completed.

