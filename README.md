# Calvin Editor

GUI Editor to be used as the main interface with the Calvin Engine.

Currently configured to run the imgui GLFW+Vulkan example.

# Building
## Dependencies
* Vulkan 1.3
* GLFW3
* imgui (added as a `meson wrap`)

We currently only support the `meson` build system, if you want to use a different system, you'll need to procure your own version of `imgui` as `meson` is used to download it.

Setup your project:
```sh
meson setup build_dir source_dir
```

To compile, just run `ninja` directly.
```sh
ninja -C build_dir
```

