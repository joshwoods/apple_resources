

- Core ML
- MLModelCollection
-  endAccessing(identifier:) Deprecated

Type Method

# endAccessing(identifier:)

Terminates access to a model collection.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedvisionOS 1.0–1.1Deprecated

``` source
class func endAccessing(identifier: String) async throws -> Bool
```

Deprecated

Use Background Assets or URLSession instead.

## Parameters 

`identifier`  

The name of the model collection.

## Discussion

Use this method when your app no longer needs access to a model collection.

- Swift
- Objective-C

```
MLModelCollection.endAccessing(identifier: modelCollectionName) { result in
    switch result {
    case .success():
        print("Successfully ended access to `\(modelCollectionName)`.")

    case .failure(let error):
        print("Error ending access to `\(modelCollectionName)`: \(error)")
    }
}
```

```
[MLModelCollection endAccessingModelCollectionWithIdentifier:modelCollectionName
                                           completionHandler:^(BOOL success,
                                                               NSError * _Nullable error) {
    if (success) {
        NSLog(@"Successfully ended access to `%@`.", modelCollectionName);
    }
    else {
        NSLog(@"Error ending access to `%@`: %@", modelCollectionName, error);
    }
}];
```

