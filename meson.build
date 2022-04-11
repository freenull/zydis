project(
  'zydis',
  'c',
  version: '4.0.0.0',
  license: 'MIT',
  subproject_dir: 'dependencies'
)

zycore = subproject('zycore')
zycore_lib_dep = zycore.get_variable('zycore_lib_dep')

includes = include_directories('include')
subdir('src')

pkg_mod = import('pkgconfig')
pkg_mod.generate(
  zydis_lib,
  version: '4.0.0.0',
  name: 'libzydis',
  filebase: 'zydis',
  description: 'Zydis disassembler'
)
