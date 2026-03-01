brew update
brew install gcc 
brew install boost
brew install tbb
brew install openblas
brew install --build-from-source dlib
brew install wget
brew install opencv

# Build 
mkdir -p build && cd build
cmake -D WITH_OPENMP=ON -D CMAKE_BUILD_TYPE=Release ..
make
