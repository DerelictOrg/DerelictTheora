DerelictOgg
==========

A dynamic binding to [libtheora][1] for the D Programming Language.

For information on how to build DerelictTheora and link it with your programs, please see the post [Using Derelict][2] at the The One With D.

For information on how to load the libtheora library via DerelictTheora, see the page [DerelictUtil for Users][3] at the DerelictUtil Wiki. In the meantime, here's some sample code.

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
    // Load the base codec library;
    DerelictTheora.load();

    // Load the libtheoradec library for decoding a video
    DerelictTheoraDec.load();

    // Load the libtheoraenc library for encoding a video
    DerelictTheoraEnc.load();

    // Now libtheora functions can be called.
    ...
}
```

[1]: http://xiph.org/theora/
[2]: http://dblog.aldacron.net/derelict-help/using-derelict/
[3]: https://github.com/DerelictOrg/DerelictUtil/wiki/DerelictUtil-for-Users
