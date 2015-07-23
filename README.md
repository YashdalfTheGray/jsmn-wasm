# JavaScript MN - Web Assembly July 22, 2015

## DigitalCamp.us

Some sort of initiative targetted towards IT and inhiring instead of outsourcing. They also want to tap into meetup groups to support this kind of thing. 

How do you engage Native American population into IT...for whatever reason.

## WebAssembly

### Keywords

* WebGl
* asm.js
* emscripten
* WebAssembly

### [Angry Bots](http://beta.unity3d.com/jonas/AngryBots/)

This game was created using asm.js (and also unity3d) which is just WebAssembly on steroids. 

### WebGL 

WebGL is OpenGL for the web. It's open-source, royalty-free and cross-platform. It uses low-level calls directly to the GPU. 

It's not for the faint of heart. 

WebGL support can be looked at by going to [CanIUse](http://www.caniuse.com/webgl) or checking [browser support](http://get.webgl.org).

### ASM.js and WebAssembly

ASM is not garbage collected or interpretted. It should be used for something that's CPU intensive, games, video processing and things of that nature. 

You can write code in any language if there is a transpiler that can take it down to highly optimized javscript. 

Enscripten is an LLVM based tool that takes C or C++ code and turns it into the JavaScript code mentioned above. Then this code can be run using asm.js which is a polyfill that can be pulled in. 

WebAssembly is expected to be an optimized, agreed upon standards-based implementation of ASM.js

Luke Wagner annouced WebAssembly on the mozilla blog and there is something up on [Github](https://github.com/WebAssembly/design). Basically, they want to deliver something that can be natively decoded and parsed and be done very quickly. 

If you compile asm.js "programs" into WebAssembly, the size can be reduced by about 60%. Most languages are going to be supported but for now it's only C/C++. JavaScript compilation to WebAssembly will also be supported at some point. 

WebAssembly is not supposed to replace JavaScript, it is designed to complement JavaScript. It will use compiled C++ apps (binary executables) and use JavaScript as the glue. 

Brenden Eich, on his [website](http://www.brendeneich.com), has a video about ECMAScript Harmony and the rise of compilers. He talks about the ES versions and the cadence of releases. People are also using transpilers and compilers to get support for newer standards.

Check out [Dead Trigger 2](http://beta.unity3d.com/jonas/DT2/) on Unity3D. It features MACHINE GUN CHICKEN SENTRIES!

## Innovation vs. Impatience

Slide deck courtesy of @codepo8

The deck talks mainly about JavaScript including the limitations of the language and the platform. JavaScript is not foolproof yet, people use it but not everyone can or wants to. 

"The web is not defined by technological availability."

Ultimately, JavaScript is not the greatest solution for the web. HTML and CSS are fault-tolerant, JavaScript is not. 

The community is impatient so polyfills are written and used. The issue becomes when no one pulls out the polyfills. This leads to people being dependant on (and only knowing about) polyfills and transpilers. 

Mobile detection is a mess because agent strings are insane. It's all about 'if it ain't broke, don't fix it' mentality. 

Browser innovation is slow and JavaScript is being used for a lot more than what it was meant to do so developers just deal with it and come up with shims, code duct tape to layer over. At some point it becomes duct tape over duct tape. 

## Compiling C into JavaScript

1. Write something in C.
2. Use emscripten to compile the C code into a web binary. Use `emcc file.c -o file.js` to create a node.js runnable JavaScript. Use `emcc file.c -o file.html` to create something that can be pulled up in a web browser. 

Just like `"use strict"`, some browsers also support `"use asm"` if they support the speedier optimizations. This can be used to get to the more optimized JavaScript. 
