# Dockerised MPQ Extractor

![Stars](https://img.shields.io/docker/stars/nicolaw/trinitycore.svg) ![Pulls](https://img.shields.io/docker/pulls/nicolaw/trinitycore.svg) ![Build](https://img.shields.io/docker/automated/nicolaw/trinitycore.svg) ![Build](https://img.shields.io/docker/build/nicolaw/trinitycore.svg)

MPQ extractor build environment and wrapper.


## Todo

This is a work-in-progress.

    docker build -t mpqextractor . \
      && docker run -it \
          -v $PWD/artifacts:/artifacts \
          -v $PWD/source:/usr/local/src \
          -v $PWD/../../World_of_Warcraft:/World_of_Warcraft \
          mpqextractor
    
    LD_LIBRARY_PATH=./artifacts/bin ./artifacts/bin/MPQExtractor


## License

MIT License

Copyright (c) 2017 Nicola Worthington <nicolaw@tfb.net>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

