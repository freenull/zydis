zydis_sources = [
  'Decoder.c',
  'DecoderData.c',
  'Encoder.c',
  'EncoderData.c',
  'Formatter.c',
  'FormatterATT.c',
  'FormatterBase.c',
  'FormatterBuffer.c',
  'FormatterIntel.c',
  'MetaInfo.c',
  'Mnemonic.c',
  'Register.c',
  'SharedData.c',
  'String.c',
  'Utils.c',
  'Zydis.c',
]

zydis_lib = library(
  'zydis',
  zydis_sources,
  dependencies: zycore_lib_dep,
  include_directories: includes,
  install: true
)

zydis_lib_dep = declare_dependency(
  include_directories: includes,
  link_with: zydis_lib
)
