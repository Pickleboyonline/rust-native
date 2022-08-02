# rust-native ⚡️
A React Native like framework that uses Rust instead of Javascript

### Why?
Because of Rust's hype and blazingly fast speed. Also, I have Typescript/Javascript fatigue. Oh yeah, and Rust apparantly has the best-in-class memory safety and developer experience.

### General Notes
 - SolidJs like reactivity and structure. The choice here is mainly because I could not find a good VDOM library in Rust.
 - In general should borrow a lot from the new react native architecture, outlined (here)[https://reactnative.dev/architecture/overview].
   We should be able to use Yoga, the flexbox engine, since its based in C/C++. Frabric can be built in Rust but instead of a VDOM
   we use obersivable reactivity to update Native UIs.
 - Should be able to be used on any platform similar to React Native's architecture. The native C bindings for iOS and Android should be
   refactored into standard modules that can be called.
   
### Main Simplified Goal
 - Build the classic React Native counter example using this framework.

### Milestones
 - [ ] Build an app that can print "hello world!" in the console.
 - [ ] Mount a view from Rust
 - [ ] Display a hello world app but with a centered text on display
 - [ ] Integrate reactivity into the app with hooks and the like
 - [ ] Create/extend macros that manage views and bind methods similar to react.
 - [ ] Add styling.
 - [ ] hot reloading (hard)

### Interesting Links
 - https://github.com/arctic-hen7/perseus
   SolidJS framework for wasm.
 - https://github.com/sycamore-rs/sycamore
   Reactivity library in Rust
