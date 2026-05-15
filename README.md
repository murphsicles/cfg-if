# @std/cfg-if — Conditional Compilation Macro for Zeta

Auto-converted from [cfg-if](https://crates.io/crates/cfg-if) v1.0.4 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **cfg_if!** — ergonomic conditional compilation similar to `if/else if/else` chains
- **Compile-time** — evaluated at compile time, dead branches are eliminated
- **Composable** — supports nested cfg_if! blocks

## Usage
```zeta
use @std/cfg_if::cfg_if;

cfg_if! {
    if #[cfg(target_os = "linux")] {
        println!("Running on Linux");
    } else if #[cfg(target_os = "macos")] {
        println!("Running on macOS");
    } else {
        println!("Running on an unknown OS");
    }
}
```

## Stats: 1 file, 41 lines, 0 unsupported items

## License: MIT