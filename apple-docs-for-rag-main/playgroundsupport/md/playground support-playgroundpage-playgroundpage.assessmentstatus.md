

- Playground Support
- PlaygroundPage
-  PlaygroundPage.AssessmentStatus 

Enumeration

# PlaygroundPage.AssessmentStatus

The values you use to communicate whether a learner has passed, failed, or not yet finished the task on a page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundPage.AssessmentStatus
```

## Topics

### Passing

case pass(message: String?)

An assessment that communicates that a learner has successfully completed a task.

### Failing

case fail(hints: [String], solution: String?)

An assessment that communicates that a learner hasn't successfully completed a task.

## See Also

### Assessing Progress

var assessmentStatus: PlaygroundPage.AssessmentStatus?

A value that indicates whether a learner has passed, failed, or not yet finished the task on a page.

