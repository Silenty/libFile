cmake_minimum_required(VERSION 2.6) # Pour éviter un warning au lancement de CMake, on doit préciser la version minimale

# Nom du projet
project(libAdvancedFiles)

include_directories(
)

link_directories(
)

SET(EXECUTABLE_OUTPUT_PATH ../bin/)


file(
    GLOB_RECURSE
    source_files
    src/*
)

# Déclaration de l'exécutable
add_executable(
    test
    ${source_files}
)

target_link_libraries(
        test
)


