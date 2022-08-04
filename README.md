# rust-native ⚡️

A React Native like framework that uses Rust instead of Javascript

### Why?

Because of Rust's hype and blazingly fast speed. Also, I have Typescript/Javascript fatigue. Oh yeah, and Rust apparently has the best-in-class memory safety and developer experience.

### General Notes

- SolidJs like reactivity and structure. The choice here is mainly because I could not find a good VDOM library in Rust.
- **[NEW]**: Might convert this project into a Rust version of https://kotlinlang.org/lp/mobile/. After looking at SwiftUI and
  Android's Jetpack Compose, the new mobile APIs look so similar to React I think it's pointless to rewrite everything in Rust when the
  native alternatives are so good now.

  I believe what would be more useful is to share logic between iOS and Android, similar to share a Redux store in the native language.
  Rust can offer advantages over native kotlin when it comes to performance.

- In general should borrow a lot from the new react native architecture, outlined (here)[https://reactnative.dev/architecture/overview].
  We should be able to use Yoga, the flexbox engine, since its based in C/C++. Fabric can be built in Rust but instead of a VDOM
  we use observable reactivity to update Native UIs.
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

- https://github.com/vislyhq/stretch

  Flexbox

- https://github.com/MoAlyousef/floui-rs and https://github.com/MoAlyousef/floui

  iOS and Android Rust Widgets

- https://medium.com/visly/rust-on-ios-39f799b3c1dd

  Rust on iOS and Android

- https://reactnative.dev/architecture/overview

- https://chinedufn.github.io/percy/html-macro/classes/index.html

  Rust VDOM, could be useful for writing macros

- https://github.com/rustwasm/wasm-bindgen

  Inspiration for https://github.com/nvzqz/swift-bindgen

- https://mozilla.github.io/uniffi-rs/Overview.html

  This module can effectively serve as our "Bridge" between Kotlin, Swift, and Rust
  Looks to make creating bindings way easier than by hand and should be able to integrate into the
  IDE

- https://github.com/thombles/dw2019rust
- https://source.android.com/setup/build/rust/building-rust-modules/overview
- https://bazel.build/tutorials/ios-app

### Documentation

We use [docusaurus](https://docusaurus.io/) for documentation. Please update the markdowns accordingly

### TODOs:

- [ ] Implement Github Actions to auto compile docs on main branch change.
- [ ] Learn basic Rust
- [ ] Create a Rust monorepo

### Project File Structure
