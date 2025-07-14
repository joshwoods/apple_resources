

- Playground Support
- PlaygroundPage
- PlaygroundPage.AssessmentStatus
-  PlaygroundPage.AssessmentStatus.pass(message:) 

Enumeration Case

# PlaygroundPage.AssessmentStatus.pass(message:)

An assessment that communicates that a learner has successfully completed a task.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case pass(message: String?)
```

## Parameters 

`message`  

A message you use to affirm a learner's succes.

## Discussion

The `message` associated value can contain markup. For more information on markup, see Markup Formatting Reference. The example below shows a popover with the message “**Great** job!”

PlaygroundPage.current.assessmentStatus = .pass(message: &quot;**Great** job!&quot;)

