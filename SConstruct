cpp_flags = Split('''-std=c++1y 
                     -O0 
                     -g''')

build_env = Environment(CXXFLAGS = cpp_flags)   

VariantDir('_build', 'src', duplicate=0)

main_program = ['_build/Main.cc', '_build/IO.cc']
executable = '_out/RunMe'
build_env.Program(source = main_program, target = executable)