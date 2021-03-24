project('dolly', 'c', default_options : ['c_std=gnu99', 'warning_level=2'])
common_src = files('files.c', 'dollytab.c', 'movebytes.c','resolve.c','transmit.c')
incdir = include_directories('.')
deps =  declare_dependency(
  include_directories : incdir 
  )

dolly = executable(
  'dolly',
  'dolly.c', common_src,
  dependencies : deps,
  install : true,
  install_dir : get_option('bindir')
)
