RNNoise is a noise suppression library based on a recurrent neural network.

To install autoconf `sudo apt-get install autoconf`

To install libtool `sudo apt-get install libtool`


To compile, just type:
% ./autogen.sh
% emconfigure ./configure
% emmake make

Optionally:
% make install

While it is meant to be used as a library, a simple command-line tool is
provided as an example. It operates on RAW 16-bit (machine endian) mono
PCM files sampled at 48 kHz. It can be used as:

./examples/rnnoise_demo <noisy speech> <output denoised>

The output is also a 16-bit raw PCM file.

The latest version of the source is available from
https://gitlab.xiph.org/xiph/rnnoise .  The github repository
is a convenience copy.

For Dumping "hdf5" model in "c"

```cd training```
```python dump_rnn.py {MODEL_NAME}.hdf5 rnn_data.c rnn_data.txt```
