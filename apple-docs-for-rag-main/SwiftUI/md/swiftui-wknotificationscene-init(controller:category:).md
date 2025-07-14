

- SwiftUI
- WKNotificationScene
-  init(controller:category:) 

Initializer

# init(controller:category:)

Creates a scene that appears in response to receiving a specific category of remote or local notifications.

watchOS 7.0+

``` source
init(
    controller: Controller.Type = Controller.self,
    category: String
)
```

## Parameters 

`controller`  

The type of WKUserNotificationHostingController to display upon receipt of the specified notification category.

`category`  

The category of notifications to listen for.

## Discussion

Use a watch notification instance to add support for one or more Apple Watch notification scenes that appear on receipt of the local or remote notification categories you specify. The example below, adds two notification scenes to the app declaration:

```
@main
struct PopQuizApp : App {
    var body: some Scene {
        MainScene {
            RootView()
        }

        WKNotificationScene(
            controller: QuizTimeController.self,
            category: "com.example.quiztime"
        )

        WKNotificationScene(
            controller: QuizResultsController.self,
            category: "com.example.results"
        )
    }
}
```

Each WKNotificationScene declaration references a WKUserNotificationHostingController and a category string that you provide. The hosting controller displays your notification’s content view upon receipt of a local or a PushKit notification. The category string you specify corresponds to the category name in the notification’s dictionary and describes a specific notification that contains the content displayed by the notification view.

