DerelictTheora
==========

A dynamic binding to [libtheora][1] for the D Programming Language.

Please see the pages [Building and Linking Derelict][2] and [Using Derelict][3], in the Derelict documentation, for information on how to build DerelictTheora and load libtheora at run time. In the meantime, here's some sample code.

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
[2]: http://derelictorg.github.io/compiling.html
[3]: http://derelictorg.github.io/using.html