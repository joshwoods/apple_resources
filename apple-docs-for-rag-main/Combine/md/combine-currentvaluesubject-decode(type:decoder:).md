

- Combine
- CurrentValueSubject
-  decode(type:decoder:) 

Instance Method

# decode(type:decoder:)

Decodes the output from the upstream using a specified decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func decode(
    type: Item.Type,
    decoder: Coder
) -> Publishers.Decode where Item : Decodable, Coder : TopLevelDecoder, Self.Output == Coder.Input
```

## Parameters 

`type`  

The encoded data to decode into a struct that conforms to the Decodable protocol.

`decoder`  

A decoder that implements the TopLevelDecoder protocol.

## Return Value

A publisher that decodes a given type using a specified decoder and publishes the result.

## Discussion

Use decode(type:decoder:) with a JSONDecoder (or a PropertyListDecoder for property lists) to decode data received from a URLSession.DataTaskPublisher or other data source using the Decodable protocol.

In this example, a PassthroughSubject publishes a JSON string. The JSON decoder parses the string, converting its fields according to the Decodable protocol implemented by `Article`, and successfully populating a new `Article`. The Publishers.Decode publisher then publishes the `Article` to the downstream. If a decoding operation fails, which happens in the case of missing or malformed data in the source JSON string, the stream terminates and passes the error to the downstream subscriber.

```
struct Article: Codable {
    let title: String
    let author: String
    let pubDate: Date
}

let dataProvider = PassthroughSubject()
cancellable = dataProvider
    .decode(type: Article.self, decoder: JSONDecoder())
    .sink(receiveCompletion: { print ("Completion: \($0)")},
          receiveValue: { print ("value: \($0)") })

dataProvider.send(Data("{\"pubDate\":1574273638.575666, \"title\" : \"My First Article\", \"author\" : \"Gita Kumar\" }".utf8))

// Prints: ".sink() data received Article(title: "My First Article", author: "Gita Kumar", pubDate: 2050-11-20 18:13:58 +0000)"
```

## See Also

### Encoding and Decoding

func encode&lt;Coder>(encoder: Coder) -> Publishers.Encode&lt;Self, Coder>

Encodes the output from upstream using a specified encoder.

