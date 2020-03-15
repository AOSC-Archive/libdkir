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

library('dkir', libdkir_srcs, dependencies: libdkir_deps, install: true)
