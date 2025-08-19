# allrole-agent1  

A simple **WebAssembly (WASM)** project.  
This repository contains a minimal example module that exports a function `add(a: i32, b: i32) -> i32`.  

## Files
- **`module.wat`** → WebAssembly Text Format (source code).  
- **`agent.wasm`** → Compiled binary (WebAssembly module).  
- **`compile-and-test.sh`** → Script to compile `.wat` into `.wasm` and run a quick test.  
- **`README.md`** → Documentation for this project.  

## How to Build
1. Install [WABT (WebAssembly Binary Toolkit)](https://github.com/WebAssembly/wabt)  
   - macOS: `brew install wabt`  
   - Linux (Ubuntu/Debian):  
     ```bash
     sudo apt-get update
     sudo apt-get install wabt
     ```
2. Compile the `.wat` into `.wasm`:  
   ```bash
   wat2wasm module.wat -o agent.wasm
