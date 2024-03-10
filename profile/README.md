# `witer`

## An iterator-based Win32 window library built in Rust

[![Crates.io Version](https://img.shields.io/crates/v/witer)](https://crates.io/crates/witer)
[![Discord](https://img.shields.io/discord/1215348294105169940?logo=discord&label=discord&color=5865F2)](https://discord.gg/KEtfte9xWZ)

```rust
use witer::prelude::*;

fn main() {
  // Configure
  let settings = WindowSettings::default();

  // Build
  let window = Window::new(settings).unwrap();

  // Run
  for message in &window {
    if let Message::Window(..) = message {
      println!("{message:?}");
    }
  }
}
```

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
