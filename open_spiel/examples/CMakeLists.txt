add_executable(benchmark_game benchmark_game.cc ${OPEN_SPIEL_OBJECTS})
add_test(benchmark_game_test benchmark_game --game=tic_tac_toe --sims=100 --attempts=2)

add_executable(example example.cc ${OPEN_SPIEL_OBJECTS})
add_test(example_test example --game=tic_tac_toe --seed=0)

add_executable(matrix_example matrix_example.cc ${OPEN_SPIEL_CORE_OBJECTS})
add_test(matrix_example_test matrix_example)

add_executable(mcts_example mcts_example.cc ${OPEN_SPIEL_OBJECTS})
add_test(mcts_example_test mcts_example)

add_executable(value_iteration_example value_iteration_example.cc ${OPEN_SPIEL_OBJECTS})
add_test(value_iteration_example_test value_iteration_example)

add_executable(cfr_example cfr_example.cc ${OPEN_SPIEL_OBJECTS})
add_test(cfr_example_test cfr_example)

add_executable(gtp gtp.cc ${OPEN_SPIEL_OBJECTS})
