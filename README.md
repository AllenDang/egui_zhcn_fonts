# egui_zhcn_fonts

Loads simplified chinese fonts to egui, currently works for windows/macos/linux.

## Installation

Add to your `Cargo.toml`:

```toml
[dependencies]
egui_zhcn_fonts = "0.1"
```

## Usage

Basic usage:

```rust
struct App {
  data:String
}

impl App {
  pub fn new(cc: &eframe::CreationContext<'_>) -> Self {
    // Add this to your app's initialize
    egui_zhcn_fonts::add_sys_ui_fonts(&cc.egui_ctx);

    Self {
      data: "你好啊"
    }
  }
}
```

## Compatibility egui versions

| egui_zhcn_fonts | Egui |
| --------------- | ---- |
| 0.1             | 0.31 |

## Supported Platforms

### macOS

- Loads "PingFang" and "Songti"

### Windows

- Loads "MSYH"

### linux

- Loads "wqy-microhei" and "SourceHanSansCN"

## Contributing

Contributions are welcome! Please open an issue or PR for:

- Platform-specific enhancements

## License

MIT/Apache
