

- Core Animation
- CAEmitterCell
-  emitterCells 

Instance Property

# emitterCells

An optional array containing the sub-cells of this cell.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var emitterCells: [CAEmitterCell]? { get set }
```

## Discussion

When specified, each particle emitted by the cell acts as an emitter for each of the cell’s sub-cells. The emission point is the current particle position and the emission angle is relative to the current direction of the particle.

The default value of this property is `nil`.

The following code shows how you can create a firework style effect using sub-cells. The `fireworkCell` has an emission longitude of one quarter turn anti-clockwise to emit particles upwards. It emits `trailCell` instances which have a slight yAcceleration that simulates gravity.

Note that the scale and color of `fireworkCell` are inherited by `trailCell`.

Listing 1. Creating particle trails

```
let image = UIImage(named: "RadialGradient.png")!.cgImage

let emitterLayer = CAEmitterLayer()

emitterLayer.emitterPosition = CGPoint(x: 512, y: 512)

let fireworkCell = CAEmitterCell()
fireworkCell.color = UIColor.red.cgColor
fireworkCell.birthRate = 3
fireworkCell.lifetime = 10
fireworkCell.velocity = 100
fireworkCell.scale = 0.05
fireworkCell.emissionLongitude = -CGFloat.pi * 0.5
fireworkCell.emissionRange = -CGFloat.pi * 0.25
fireworkCell.contents = image

let trailCell = CAEmitterCell()
trailCell.yAcceleration = 20
trailCell.birthRate = 10
trailCell.lifetime = 3
trailCell.contents = image

fireworkCell.emitterCells = [trailCell]
emitterLayer.emitterCells = [fireworkCell]

view.layer.addSublayer(emitterLayer)
```

## See Also

### Providing Emitter Cell Content

var contents: Any?

An object that provides the contents of the layer. Animatable.

var contentsRect: CGRect

A rectangle (in the unit coordinate space) that specifies the portion of contents that the receiver should draw. Animatable.

