project('uWebSocket', 'cpp')

comp_flags = ['-std=c++11']
link_flags = ['-lssl', '-lz', '-lcrypto']

includes = include_directories('src')
subdir('src')

sources_dep = declare_dependency(include_directories: includes,
sources: sources)

shared_library('uWS', sources, 
              cpp_args: comp_flags, 
              link_args: link_flags)
