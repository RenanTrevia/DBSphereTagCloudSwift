# SwiftNum
*SwiftNum* is an in-progress numerical computing library in Swift. It uses Accelerate / BLAS, so it should be quite fast.

Currently SwiftNum only support macOS, but Linux support shouldn't be too hard, and is planned.

## So What does SwiftNum Do?
**SwiftNum aims to provide a clean, easy and efficient Swift interface for common numerical computing tasks.**

So far, **SwiftNum** has implemented:
- [Linear Algebra](https://github.com/donald-pinckney/SwiftNum/tree/master/Sources/Linear)
- [Optimization Routines](https://github.com/donald-pinckney/SwiftNum/tree/master/Sources/Optimization)
  - [Gradient Descent](https://en.wikipedia.org/wiki/Gradient_descent)
  - [Conjugate Gradient Method](https://en.wikipedia.org/wiki/Conjugate_gradient_method)
- [Signal Processing: FFT and Windowing](https://github.com/donald-pinckney/SwiftNum/tree/master/Sources/SignalProcessing)
- [Plotting](https://github.com/donald-pinckney/SwiftNum/tree/master/Sources/Plotting): Just makes calls to *gnuplot*, but is very convenient from Swift.

## Requirements
Currently the requirements are:
- macOS
- Swift 4.0.x
- *gnuplot* installed if you wish to plot, though **SwiftNum** will build without it.

## How to Use
Just add it is a dependency to your `Package.swift` file:
```swift
.Package(url: "https://github.com/donald-pinckney/SwiftNum", Version(1, 9, 9))
```
