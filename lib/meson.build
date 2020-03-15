libdkir_deps = [
  dependency('gee-0.8'),
  dependency('json-glib-1.0'),
]

libdkir_srcs = files(
  'ir.vala',
  'partitioninfo.vala',
  'extractinfo.vala',
  'configinfo.vala',
  'userinfo.vala',
  'overrideinfo.vala',
  'bootloaderinfo.vala',
)

# The [true, true, true] in install_dir tells meson to install the generated
# VAPI file and C header file. See:
# https://mesonbuild.com/Vala.html#changing-c-header-and-vapi-names
library(
  'dkir',
  libdkir_srcs,
  dependencies: libdkir_deps,
  install: true,
  install_dir: [true, true, true],
)
