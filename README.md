# SimpleImageProcessing

SimpleImageProcessing is a Swift framework that provides developers with a set of image processing tools.

It includes such categories:
- Utilities functions (Image view based on Metal, Camera stream helpers);
- Convolution filters (Gaussian blur, Box blur..);
- Operators (Sobel Operator, Scharr Operator..);
- Texture/noise generators (Voronoi noise, Perlin noise..).

## Installation

You may use the framework by downloading it and adding to your project.
No additional actions needed.

Complete the following steps:

1. Download the Framework directly from Github
2. Paste it to your Xcode project
3. In Project settings select to Embed the framework.

## Usage

After installing the framework, you can import the module by adding the following line in the "header" of any of your swift files:
```swift
import SimpleImageProcessing
```
To use framework filters or generators you can use provided classes
```swift
let filter = Grayscale()
filter.inputImage = image
let output = filter.outputImage
```
```swift
let simplex = SimplexNoiseGenerator()
simplex.extent = someExtent
let output = simplex.outputImage
```

