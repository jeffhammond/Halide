CXX = c++
CXXFLAGS = -O3 -std=c++17
HALIDE_PATH = /opt/halide

all: lesson_01_basics.exe lesson_02_input_image.exe lesson_03_debugging_1.exe lesson_04_debugging_2.exe lesson_05_scheduling_1.exe lesson_06_realizing_over_shifted_domains.exe lesson_07_multi_stage_pipelines.exe lesson_08_scheduling_2.exe lesson_09_update_definitions.exe lesson_10_aot_compilation_generate.exe lesson_10_aot_compilation_run.exe lesson_11_cross_compilation.exe lesson_12_using_the_gpu.exe lesson_13_tuples.exe lesson_14_types.exe lesson_15_generators.exe lesson_16_rgb_generate.exe lesson_16_rgb_run.exe lesson_17_predicated_rdom.exe lesson_18_parallel_associative_reductions.exe lesson_19_wrapper_funcs.exe lesson_20_cloning_funcs.exe lesson_21_auto_scheduler_generate.exe lesson_21_auto_scheduler_run.exe

%.exe: %.cpp
	${CXX} ${CXXFLAGS} -I${HALIDE_PATH}/include $< -o $@ -L${HALIDE_PATH}/lib -lhalide

clean:
	-rm -f *.o
	-rm -f *.exe
	-rm -rf *.dSYM
