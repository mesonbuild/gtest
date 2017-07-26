incdir = include_directories('include', '.')
libsources = files('src/gmock-all.cc')
mainsources = files('src/gmock_main.cc')

gmock_mainless_dep = declare_dependency(
	include_directories : incdir,
	sources :  libsources,
	dependencies : dependency('threads')
)

gmock_with_main_dep = declare_dependency(
	include_directories : incdir,
	sources :  [libsources,mainsources],
	dependencies : dependency('threads')
)
