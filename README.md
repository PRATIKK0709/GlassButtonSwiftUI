# GlassButtonSwiftUI


This project demonstrates how to create a glass effect button with a blue gradient background using SwiftUI. The glass effect button is created with the help of the `BlurView` and `GlassButton` components.

## Getting Started

### Prerequisites

- Xcode (12.0 or later)
- Swift (5.0 or later)

### Installation

1. Clone this repository to your local machine or download the source code.
2. Open the project in Xcode.

## Usage

The `GlassButton` component provides a customizable glass button with a label and an action closure.

```swift
struct GlassButton: View {
    var label: String
    var action: () -> Void

    var body: some View {
        // Button styling code
    }
}
```

The `BlurView` component creates a blur effect for the background of the button.

```swift
struct BlurView: UIViewRepresentable {
    let style: UIBlurEffect.Style

    func makeUIView(context: Context) -> UIVisualEffectView {
        let view = UIVisualEffectView(effect: UIBlurEffect(style: style))
        return view
    }

    func updateUIView(_ uiView: UIVisualEffectView, context: Context) {
    }
}
```

The `GlassButtonDemo` view sets up a gradient background and places the `GlassButton` on it.

```swift
struct GlassButtonDemo: View {
    var body: some View {
        // Code to set up the gradient background and button
    }
}
```


## Customization

You can customize the appearance of the GlassButton by adjusting the blur style, corner radius, opacity, colors, and other properties to suit your design preferences.
