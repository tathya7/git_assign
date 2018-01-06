# Valgrind Exercise

## Standard install via command-line
```bash
# Configure the project and generate a native build system:
  # Must re-run this command whenever any CMakeLists.txt file has been changed.
  cmake -S ./ -B build/
# Compile and build the project:
  # rebuild only files that are modified since the last build
  cmake --build build/
  # or rebuild everything from scracth
  cmake --build build/ --clean-first
  # to see verbose output, do:
  cmake --build build/ --verbose
# Run test:
  ctest --test-dir build/
  # to filter the output to show only certain tests
  ctest --test-dir build/ -R any_key_word_to_filter
# Clean
  cmake --build build/ --target clean
# Clean and start over:
  rm -rf build/
```

