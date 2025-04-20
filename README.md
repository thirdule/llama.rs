# 🦙 llama.rs

Rust workspace for building a modular integration and runtime layer around `llama.cpp`.

## Workspace Structure

```
llama.rs/
├── llama-core/      # (Optional) Rust-native tensor and memory operations (ggml-style)
├── llama-sys/       # FFI bindings to C/C++ functions from llama.cpp (via `cc`)
├── llama-model/     # Responsible for GGUF parsing, tokenizer, vocabulary loading
├── llama-runtime/   # High-level execution API, wraps llama-core + model loading
├── llama-cli/       # Example CLI application that runs inference
└── examples/        # (Optional) Additional Rust examples and integration tests
```

## Getting Started

```bash
cargo build --workspace
cargo run -p llama-cli
```

## License

Apache 2.0 License
