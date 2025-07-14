

- Swift Playgrounds
-  Adding a Swift package to your app playground 

Article

# Adding a Swift package to your app playground

Extend the functionality of your app playground by finding and adding a publicly available Swift package.

## Overview

Swift packages solve the problem of sharing code and resources between projects — and with other developers. You can use the same code in more than one playground without having to maintain multiple copies. You can write a powerful app without having to write it all yourself building on work shared by others.

Swift packages are portable containers for code and resources that your app playground can access by URL in Xcode or in Swift Playgrounds. Apple provides a selection of Swift packages on GitHub that you can link to from your app playgrounds. Swift Playgrounds uses the Swift Package Manager to locate, download, and integrate all the packages included in your app playground.

As an example, you’ll use the Deck of Playing Cards Swift package. This package includes Swift code that describes a deck of playing cards that you’ll use to build a card game in SwiftUI. The `DeckOfPlayingCards` package includes enumerations and functions for the playing cards, including their rank (numbered 2 through 10, Jack, Queen, King, and Ace) and suit (clubs, diamonds, hearts, and spades), and functions for shuffling and dealing the cards.

To add the URL to your app playground:

1.  Tap or click the Add Document button (+) in the toolbar above the project navigator.

2.  Tap or click the menu and choose Swift Package.

3.  In the text field that appears, enter the URL for the Swift package to use in your app playground, then tap or click Return.

Swift Playgrounds uses the Swift Package Manager to locate the requested package, including details like the package version and what functionality the package offers.

The `DeckOfPlayingCards` package provides a single product. Select it with the toggle switch in the figure below and tap or click “Add to Project”. Then Swift Package Manager downloads the selected version. The `DeckOfPlayingCards` package appears in the Packages section of the project navigator below your code.

With the Swift package added to your app playground, you’ll need to import its code and resources for use in your own code. The `DeckOfPlayingCards` package contains two modules – pieces of functionality – of interest for this sample, the `PlayingCard` and `DeckOfPlayingCards` modules. You can review the code for `DeckOfPlayingCards` in the `Deck` file in the package’s `DeckOfPlayingCards` source directory in the Project navigator. The `Deck` code contains the following functions:

- `standard52CardDeck()` — Specifies a standard 52 card deck.

- `shuffle()` — Reorders the cards in the deck.

- `deal()` — Removes the last card in the deck returning it to the caller.

The playing card drawing app playground’s `ContentView` implementation imports `PlayingCard` and `DeckOfPlayingCards`. When SwiftUI calls the `body` property in the `ContentView`, the `ContentView` calls the `hand()` function. `hand()` creates and shuffles a standard 52 card deck and returns an array of the last three cards, “dealing” them to the `ContentView` for display. These three cards are passed to a custom `CardView` for drawing to the screen.

```
```

## See Also

### App playgrounds

Debugging an App Playground using the Console

Learn different methods to debug your code using console output.

Previewing SwiftUI views in Swift Playgrounds

Use the canvas in Swift Playgrounds to see a live preview of the SwiftUI views in your app.

Requesting access to capabilities for your app playground

Request access for your app to protected resources, services, or device hardware such as sensors.

Importing sample content into user app playgrounds

Learn how to bring sample code into your app playground.

