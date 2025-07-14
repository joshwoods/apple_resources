

- Playground Support
-  PlaygroundPage 

Class

# PlaygroundPage

An object you use to configure the state of a playground page and its live view.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

``` source
final class PlaygroundPage
```

## Overview

You access the current playground page by using this class's static current property; no more than one page is ever active at the same time. Playground pages in Swift Playgrounds have different capabilities than playground pages in Xcode. For example, control over the execution mode is available only in Swift Playgrounds, while the Touch Bar is accessible only to playgrounds in Xcode.

Both playground environments can set a live view, which you use to show the visual results of running the code on the playground page.

PlaygroundPage.current.setLiveView(
    List(0..&lt;42) { number in
        Text(&quot;My favorite number is \(number).&quot;)
    }
)

You also use the current page to configure the *always-on live view*, a special live view that runs in a separate process from the code on a playground page and is available only in Swift Playgrounds. The always-on live view can display results that persist across multiple runs of the code on a page, or that you need for one-time setup tasks that take time to run. For example, you might use the always-on live view to display multiple stages of progress through a playground page that has multiple steps to reach the solution.

Because the always-on live view is hosted outside of the process that runs the code on a playground page, you communicate with it indirectly. For more information, see Messaging Between a Playground Page and the Always-On Live View.

## Topics

### Configuring Live Views

static let current: PlaygroundPage

The current playground page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a SwiftUI view that shows the result of running the code that’s on the current page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a view that shows the result of running the code that’s on the current page.

var liveView: (any PlaygroundLiveViewable)?

A live view that shows the result of running the code that’s on the current page.

### Configuring Execution

var executionMode: PlaygroundPage.ExecutionMode

The currently selected speed for executing the code on this playground page.

enum PlaygroundPage.ExecutionMode

The available speeds for executing the code on a playground page.

var needsIndefiniteExecution: Bool

A Boolean value that indicates whether indefinite execution is enabled.

func finishExecution() -> Never

Terminates execution of the current playground page.

### Assessing Progress

var assessmentStatus: PlaygroundPage.AssessmentStatus?

A value that indicates whether a learner has passed, failed, or not yet finished the task on a page.

enum PlaygroundPage.AssessmentStatus

The values you use to communicate whether a learner has passed, failed, or not yet finished the task on a page.

### Inspecting Page Data

var text: String

The current contents of the playground page, including any user-entered text.

var keyValueStore: PlaygroundKeyValueStore

An object that persists data on a page between multiple sessions.

Deprecated

### Displaying Touch Bar Items

var liveTouchBar: NSTouchBar?

An object you use to add items to the Touch Bar of supported MacBook Pro models.

### Instance Properties

var userModuleNames: [String]

var wantsFullScreenLiveView: Bool

### Instance Methods

func getText(forSourceFile: String, inUserModule: String) -> String?

func listSourceFiles(inUserModule: String) -> [String]

func navigateTo(page: PlaygroundPage.PageNavigation)

func openApplication(withBundleIdentifier: String, iTunesItemIdentifier: Int?)

func openPlayground(withContentIdentifier: String, toPageAtIndex: Int?)

func showGlossaryEntry(named: String, at: CGRect?, in: UIView?)

### Enumerations

enum PlaygroundPage.PageNavigation

