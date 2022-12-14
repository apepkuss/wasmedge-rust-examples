# Examples of WasmEdge Rust SDK

- [Examples of WasmEdge Rust SDK](#examples-of-wasmedge-rust-sdk)
  - [Example 1: Run a wasm app from host](#example-1-run-a-wasm-app-from-host)
  - [Example 2: Call a wasm library from host](#example-2-call-a-wasm-library-from-host)
    - [Example 2-1: Use extern functions in a wasm library](#example-2-1-use-extern-functions-in-a-wasm-library)
  - [Example 3: Arguments of non-standard wasm types in wasm function](#example-3-arguments-of-non-standard-wasm-types-in-wasm-function)
  - [Example 4: Define and register a host function](#example-4-define-and-register-a-host-function)
    - [Example 4-1: Define a host function with string arguments](#example-4-1-define-a-host-function-with-string-arguments)
  - [Example 5: Define and register async host functions](#example-5-define-and-register-async-host-functions)
  - [Example 6: AI inference over WasmEdge WASI-NN Plugin (PyTroch)](#example-6-ai-inference-over-wasmedge-wasi-nn-plugin-pytroch)
  - [Example 7: Manipulate WebAssembly linear memory](#example-7-manipulate-webassembly-linear-memory)
  - [Example 8: Use WebAssembly `Table` and `FuncRef` to invoke host functions](#example-8-use-webassembly-table-and-funcref-to-invoke-host-functions)
  - [Example 9: Run wasm functions in AOT mode](#example-9-run-wasm-functions-in-aot-mode)
  - [Example 10: Set environment variables and arguments via WasmEdge `wasi` interface](#example-10-set-environment-variables-and-arguments-via-wasmedge-wasi-interface)
  - [Example 11: Multi-threaded parallel execution with memory sharing](#example-11-multi-threaded-parallel-execution-with-memory-sharing)

## Example 1: Run a wasm app from host

This example demonstrates how to create a WebAssembly application and run it as a wasm module over WasmEdge Runtime.

- [Run wasm app from host](run-wasm-app-from-host/README.md)
  - [x] Source Code
  - [x] README
  - [x] Tutorial

## Example 2: Call a wasm library from host

This example demonstrates how to define a wasm library and call the APIs exported from the wasm library in WasmEdge Runtime.

- [Call wasm library from host](call-wasm-lib-from-host/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

### Example 2-1: Use extern functions in a wasm library

This example demonstrates how to use external functions in a wasm library, and how to call such a wasm library with WasmEdge Rust SDK.

- [Call wasm library with external dependency](call-wasm-lib-with-external-deps/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 3: Arguments of non-standard wasm types in wasm function

This example demonstrates how to define wasm functions, of which the arguments are of Rust built-in types instead of WebAssembly types.

- [WasmEdge-Bindgen](wasmedge-bindgen/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 4: Define and register a host function

This example demonstrates how to define a native function as a host function with `#[host_function]` macro, and register it into a WasmEdge `Vm` and run it over WasmEdge Runtime.

- [Define host function](define-host-func/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

### Example 4-1: Define a host function with string arguments

This example demonstrates how to define a host function that takes two arguments of Rust built-in `String` or string slice type.

- [Define host function with string arguments](define-host-func-with-string-args/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 5: Define and register async host functions

This example demonstrates how to define a native async function as an async host function with `#[async_host_function]` macro, and register it into a WasmEdge `Vm` and run it over WasmEdge Runtime.

- [Define async host functions](define-async-host-func/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 6: AI inference over WasmEdge WASI-NN Plugin (PyTroch)

This example demonstrates how to perform an object detection task over WasmEdge Runtime.

- [Object detection via WASI-NN Plugin PyTorch Backend](object-detection-via-wasinn/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 7: Manipulate WebAssembly linear memory

This example demonstrates how to manipulate linear memory.

- [Manipulate linear memory](manipulate-linear-memory/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 8: Use WebAssembly `Table` and `FuncRef` to invoke host functions

This example demonstrates how to use WebAssembly `Table` and `FuncRef` together to invoke host functions.

- [Table and FuncRef](table-and-funcref/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 9: Run wasm functions in AOT mode

This example demonstrates how to generate a AOT file with WasmEdge AOT compiler, and then load the file and run the wasm function in AOT mode.

- [Use WasmEdge AOT Compiler](run-wasm-func-in-aot-mode/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 10: Set environment variables and arguments via WasmEdge `wasi` interface

This example demonstrates how to set environment variables and arguments via WasmEdge `wasi` interface.

- [Set env vars via wasi](set-env-vars-via-wasi/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial

## Example 11: Multi-threaded parallel execution with memory sharing

This example demonstrates how to use WasmEdge Rust SDK to create multiple threads to help us render [Mandelbrot set](https://en.wikipedia.org/wiki/Mandelbrot_set) in parallel, which is a compute-intensive workload. This example also present sharing the image memory between threads while rendering the image parallelly.

- [Run in multi-threaded parallel](multi-threaded-parallel/README.md)
  - [x] Source Code
  - [x] README
  - [ ] Tutorial
