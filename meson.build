project('gtest', 'cpp', version : '1.7.0', license : 'bsd')

incdir = include_directories('include', '.')
libsources = files('src/gtest-all.cc')
mainsources = files('src/gtest_main.cc')

gtest_mainless_dep = declare_dependency(
	include_directories : incdir,
	sources :  libsources,
	dependencies : dependency('threads')
)

gtest_with_main_dep = declare_dependency(
	include_directories : incdir,
	sources :  [libsources,mainsources],
	dependencies : dependency('threads')
)
