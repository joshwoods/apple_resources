

- Playground Support
- PlaygroundPage
- PlaygroundPage.AssessmentStatus
-  PlaygroundPage.AssessmentStatus.fail(hints:solution:) 

Enumeration Case

# PlaygroundPage.AssessmentStatus.fail(hints:solution:)

An assessment that communicates that a learner hasn't successfully completed a task.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case fail(
    hints: [String],
    solution: String?
)
```

## Parameters 

`hints`  

A list of hints that might help a learner pass the assessment.

`solution`  

An explicit solution to the assessment that a learner can use to get unstuck.

## Discussion

If no solution is provided, there must be at least one string in the `hints` array.

The strings for the solution and for hints can contain markup. For more information on markup, see Markup Formatting Reference. The example below sets one hint for the page. The markup in the hint string displays the word “for” in code voice.

PlaygroundPage.current.assessmentStatus = .fail(hints: [&quot;Try using a `for` loop&quot;], solution: nil)

