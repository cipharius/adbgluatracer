project('adbgluatracer', 'c', default_options : ['c_std=c11'])
shmif = dependency('arcan-shmif')
luajit = dependency('luajit')
tui = dependency('arcan-shmif-tui')
thread = dependency('threads')
cc = meson.get_compiler('c')
math = cc.find_library('m', required : false)
shared_library('adbgluatracer', 'src/adbgluatracer.c', install : true, dependencies : [shmif, tui, luajit, math, thread])
