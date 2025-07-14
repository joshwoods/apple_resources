

- RealityKit
- Reality Composer
-  Loading Reality Composer files manually without generated code 

Article

# Loading Reality Composer files manually without generated code

Load Reality Composer files that aren’t part of your Xcode project.

## Overview

Although Xcode generates loading methods for all Reality Composer files in your Xcode project, there are times when you need to load them without the benefit of those generated loader methods. This scenario can happen, for example, when loading content downloaded as part of an in-app purchase bundle from the App Store.

You can manually load scenes synchronously or asynchronously. Unless your Reality Composer scene is very small, use the asynchronous method, which loads scenes in the background. Synchronous loading occurs on the main thread, so your app may become unresponsive if you use that method to load even moderately complex scenes.

### Create a scene URL

Regardless of whether you plan to load the scene synchronously or asynchronously, the first step is to create a URL that points to the Reality file that contains the scene you want to load. Then append the name of the scene to the URL.

Here’s an example of building a URL to load a scene from a Reality file inside your app’s bundle:

```
func createRealityURL(filename: String, 
                      fileExtension: String, 
                      sceneName:String) -> URL? {
    // Create a URL that points to the specified Reality file. 
    guard let realityFileURL = Bundle.main.url(forResource: filename, 
                                               withExtension: fileExtension) else {
        print("Error finding Reality file \(filename).\(fileExtension)")
        return nil
    }

    // Append the scene name to the URL to point to 
    // a single scene within the file.
    let realityFileSceneURL = realityFileURL.appendingPathComponent(sceneName, 
                                                                    isDirectory: false)
    return realityFileSceneURL
} 
```

### Load the scene asynchronously from the URL

Entity provides the loadAnchorAsync(contentsOf:withName:) method for loading scenes asynchronously from a URL. Loading in this manner uses the Combine framework and returns an AnyCancellable object that you use to cancel scene loading.

You must maintain a strong reference to the returned AnyCancellable object until loading has completed. Otherwise, the load process cancels as soon as the returned AnyCancellable object is deallocated. To keep a strong reference to the returned AnyCancellable object, store it in an array.

This example shows how to declare an array variable in your view controller or coordinator class to hold instances of AnyCancellable:

```
var streams = [Combine.AnyCancellable]()
```

Load your scene asynchronously, storing the AnyCancellable object in that array using the store(in:) method instead of the append(_:) method. In this way, you ensure that the system won’t cancel your load operation.

This example shows how to asynchronously load a scene from a URL:

```
func loadRealityComposerSceneAsync (filename: String,
                                    fileExtension: String,
                                    sceneName: String,
                                    completion: @escaping (Swift.Result) -> Void) {

    guard let realityFileSceneURL = createRealityURL(filename: filename, fileExtension: fileExtension, sceneName: sceneName) else {
        print("Error: Unable to find specified file in application bundle")
        return
    }

    let loadRequest = Entity.loadAnchorAsync(contentsOf: realityFileSceneURL)
    let cancellable = loadRequest.sink(receiveCompletion: { (loadCompletion) in
        if case let .failure(error) = loadCompletion {
            completion(.failure(error))
        }
    }, receiveValue: { (entity) in
        completion(.success(entity))
    })
    cancellable.store(in: &streams)
}
```

Note

If you use the store(in:) method instead of append(_:), you don’t have to remove the AnyCancellable object from the array after loading has finished. When using that method, the AnyCancellable object removes itself automatically from the array once it has finished loading.

### Load the scene synchronously from the URL

Call the loadAnchor(contentsOf:withName:) method on Entity and pass in a scene URL.

```
func loadRealityComposerScene (filename: String,
                                fileExtension: String,
                                sceneName: String) -> (Entity & HasAnchoring)? {
    guard let realitySceneURL = createRealityURL(filename: filename,
                                                 fileExtension: fileExtension,
                                                 sceneName: sceneName) else {
        return nil
    }
    let loadedAnchor = try? Entity.loadAnchor(contentsOf: realitySceneURL)

    return loadedAnchor
}

```

### Load a USDZ file asynchronously

You can load USDZ files asynchronously in the background using the loadModelAsync(contentsOf:withName:) method on Entity. Asynchronous loading of USDZ files also requires the Combine framework. To receive the scene once it’s loaded, the receiving class must conform to the Subscriber protocol.

This example shows you how to conform a view controller to the Subscriber protocol so it can receive the asynchronously loaded scene:

```
extension ViewController : Subscriber {

    // loadModelAsync loads a ModelEntity, so declare 
    // that as the Input type.
    typealias Input = ModelEntity

    // If loadModelAsync fails, it returns an Error instance, 
    // so declare Error as the Failure associated-object type.
    typealias Failure = Error

    // The publisher has finished, so ask it for the result 
    // as a single item.
    func receive(subscription: Subscription) {
        subscription.request(.max(1))
    }

    // You receive the model here and assign it to a property
    // so you can use it outside of this method. 
    func receive(_ input: ModelEntity) -> Subscribers.Demand {
        // Assign to robot, a property declared in your 
        // main view-controller class
        robot = input
        return .none
    }

    // When the publisher is done - either it has sent the 
    // model or it has errored - this method is called.
    func receive(completion: Subscribers.Completion) {
        switch (completion) {
            case .failure(let error):
                print("Error loading model: \(error)")
            case .finished:
                print("Model loaded successfully")
        }
    }
}
```

Once you set up your view controller as a Subscriber, you can start loading a USDZ file as in this example:

```
let request = Entity.loadModelAsync(contentsOf: robotURL)
request.receive(subscriber: self)
```

For more information on using the Combine Framework, see Receiving and Handling Events with Combine.

### Load a USDZ file synchronously

You can also load individual 3D models from USDZ files for use in your Reality Composer scenes. This is especially useful, for example, for loading objects that you might spawn multiple times in response to user input. In that case, you don’t want the asset loaded as part of your Reality Composer scene. Instead, you want to load it separately and add it to your scene when needed.

You can load a model synchronously using the loadModel(contentsOf:withName:) function on Entity, as in this example:

```
var loadedModel: Entity?
if let theURL = Bundle.main.url(forResource: "myModel", withExtension: "usdz") {
    let loadedModel = try? Entity.loadModel(contentsOf: theURL)
}
```

## See Also

### Scene creation

Creating 3D Content with Reality Composer

Assemble assets into a dynamic 3D composition that you can add to a scene in your app, or share with AR Quick Look.

Loading Reality Composer files using generated code

Leverage automatically generated code to load scenes from Xcode.

Adding elements to a 3D scene

Add assets to your scene from Reality Composer’s library, or import custom assets.

Configuring elements in a scene

Define the appearance and behavior of objects in a scene.

Arranging elements in a scene

Manipulate objects to complete your Reality Composer scene.

Manipulating Reality Composer scenes from code

Make programmatic changes to your scenes at runtime.

Adding procedural assets to a scene

Create procedurally generated shape primitives to your Reality Composer scene.

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

