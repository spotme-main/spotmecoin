
### About
SPOTme Coin is a cryptonote-based cryptocurrency.  Besides being just plain awesome, it is now ASIC resistant with the CN-lite Varient 1 algorithm.  

### Dependencies
* GCC 4.7.3 or later     (http://gcc.gnu.org/)
* CMake 2.8.6 or later   (http://www.cmake.org/)
* Boost 1.55 or later    (http://www.boost.org/)
* MSVC 2013 (Windows only)

Step by step Windows instructions:
https://github.com/forknote/cryptonote-generator/blob/master/docs/windows-requirements-install.md

Ubuntu (tested on Ubuntu 16.04) / Mac dependencies:
```
sudo apt-get install build-essential python-dev autotools-dev libicu-dev libbz2-dev  libcurl4-openssl-dev git qt-sdk libminiupnpc-dev miniupnpc libdb-dev libdb++-dev libssl-dev bzip2-doc cmake
```

### Usage
1. Download or compile the binaries
2. Start the daemon:
```
./spotd --config-file PATH_TO_YOUR_CONFIG
```

### Configuration parameters

All fields supported:
```
seed-node=45.32.215.48:19497
seed-node=prod2.spotmecoin.com:19497
seed-node=prod3.spotmecoin.com:19497
seed-node=prod4.spotmecoin.com:19497
seed-node=prod5.spotmecoin.com:19497
seed-node=prod6.spotmecoin.com:19497
seed-node=prod7.spotmecoin.com:19497
seed-node=prod8.spotmecoin.com:19497
seed-node=prod9.spotmecoin.com:19497
seed-node=prod10.spotmecoin.com:19497


EMISSION_SPEED_FACTOR=18
DIFFICULTY_TARGET=120
CRYPTONOTE_DISPLAY_DECIMAL_POINT=11
MONEY_SUPPLY=18446744073709551615
GENESIS_BLOCK_REWARD=6087425544324152000
SYNC_FROM_ZERO=1
DEFAULT_DUST_THRESHOLD=100000
MINIMUM_FEE=100000
CRYPTONOTE_MINED_MONEY_UNLOCK_WINDOW=10
CRYPTONOTE_BLOCK_GRANTED_FULL_REWARD_ZONE=100000
MAX_TRANSACTION_SIZE_LIMIT=100000
CRYPTONOTE_PUBLIC_ADDRESS_BASE58_PREFIX=57
DIFFICULTY_CUT_V1=60
DIFFICULTY_CUT_V2=60
DIFFICULTY_CUT=0
DIFFICULTY_LAG_V1=15
DIFFICULTY_LAG_V2=15
DIFFICULTY_LAG=0
DIFFICULTY_WINDOW_V1=720
DIFFICULTY_WINDOW_V2=720
DIFFICULTY_WINDOW=17
p2p-bind-port=19497
rpc-bind-port=19498
BYTECOIN_NETWORK=20026ce4-5b11-3d8e-78de-d00070a50b04
CRYPTONOTE_NAME=SPOT
GENESIS_COINBASE_TX_HEX=010a01ff0001c0f5d1f0faa8b8bd5402346d1a3b284587e258c5451eff42b2a439c579c9cc09920897a724381cf2013f2101580d020343890753091d1146a2afaf6b412c1151ad7bcb2db23e0e3a156119bf
MAX_BLOCK_SIZE_INITIAL=100000
UPGRADE_HEIGHT_V2=1
UPGRADE_HEIGHT_V3=30
UPGRADE_HEIGHT_V4=87000
daemon-port = 19498
bind-port = 9090
```

---


Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55.
You may download them from:
http://gcc.gnu.org/
http://www.cmake.org/
http://www.boost.org/
Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run `make'. The resulting executables can be found in build/release/src.

Advanced options:
Parallel build: run `make -j<number of threads>' instead of `make'.
Debug build: run `make build-debug'.
Test suite: run `make test-release' to run tests in addition to building. Running `make test-debug' will do the same to the debug version.
Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++' before running `make'.

On Windows:
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:
http://www.microsoft.com/
http://www.cmake.org/
http://www.boost.org/

To build, change to a directory where this file is located, and run this commands: 
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..

And then do Build.
Good luck!