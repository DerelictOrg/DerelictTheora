DerelictTheora
==========

A dynamic binding to [libtheora][1] version 1.1 for the D Programming Language.

Please see the [Derelict documentation][2], for information on how to build DerelictTheora and load libtheora at run time. In the meantime, here's some sample code.

```D
// Import all of the libtheora modules
import derelict.theora.theora;

/*
Alternatively, you can do the following:
import derelict.theora.codec;
import derelict.theora.theoraenc;
import derelict.theora.theoradec;
*/

void main() {
    // Load the libtheora codec library and its companion encoding and decoding libaries
    DerelictTheora.load();
    DerelictTheoraEnc.load();
    DerelictTheoraDec.load();

    // Now libtheora functions can be called.
    ...
}
```

[1]: http://xiph.org/theora/
[2]: https://derelictorg.github.io/