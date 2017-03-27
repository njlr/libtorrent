include_defs('//BUCKAROO_DEPS')

cxx_library(
  name = 'libtorrent',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include/libtorrent', '**/*.hpp'),
    ('include/libtorrent', '**/*.h'),
  ], prefix = 'libtorrent'),
  headers = subdir_glob([
    ('ed25519/src', '**/*.h'),
  ]),
  srcs = glob([
    'src/**/*.cpp',
    'ed25519/src/**/*.cpp',
  ]),
  compiler_flags = [
    '-std=c++14',
  ],
  visibility = [
    'PUBLIC',
  ],
  deps = BUCKAROO_DEPS,
)
