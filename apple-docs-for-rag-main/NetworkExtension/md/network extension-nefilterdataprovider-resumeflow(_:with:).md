

- Network Extension
- NEFilterDataProvider
-  resumeFlow(\_:with:) 

Instance Method

# resumeFlow(\_:with:)

Resumes a previously-paused flow.

macOS 10.15+

``` source
func resumeFlow(
    _ flow: NEFilterFlow,
    with verdict: NEFilterVerdict
)
```

## Discussion

The provider calls this method to resume a flow that the provider previously paused by returning a pause verdict.

