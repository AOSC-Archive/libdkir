valadoc = find_program('valadoc')

# Generate the package import options for valadoc
pkgs_valac = []
foreach d : libdkir_deps
  pkgs_valac += '--pkg'
  pkgs_valac += d.name()
endforeach

custom_target(
  'docs',
  build_by_default: false,
  input: libdkir_srcs,
  output: '.',
  command: [
    valadoc,
    pkgs_valac,
    '--package-name', meson.project_name(),
    '--package-version', meson.project_version(),
    '--internal',
    '--private',
    '--use-svg-images',
    '--force',
    '--basedir', meson.current_source_dir(),
    '--directory', '@OUTPUT@',
    '@INPUT@'
  ]
)
