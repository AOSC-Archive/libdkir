# DeployKit IR Parser / Emitter

This library provides an easy-to-use interface for parsing and generating the DeployKit Internal Representation (DKIR).

## Dependencies

- Runtime Dependencies
  - GLib (GObject)
  - [LibGee](https://wiki.gnome.org/Projects/Libgee)
- Build Time Dependencies
  - [The Vala Compiler](https://wiki.gnome.org/Projects/Vala)
    - To build API documentation, `valadoc` is also needed if your OS distribution does not ship it with the Vala compiler

## Build

Use [Meson](https://mesonbuild.com):

```shell
mkdir build && cd build
meson .. # Configure the project
ninja    # Build the project
```

Use Meson options to tweak the build, see [meson_options.txt](meson_options.txt).

## License

This software is licensed under the MIT license. See [COPYING](COPYING) for details.
