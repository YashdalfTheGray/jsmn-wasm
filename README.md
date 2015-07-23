# JavaScript MN - Web Assembly

## DigitalCamp.us

Some sort of initiative targetted towards IT and inhiring instead of outsourcing. They also want to tap into meetup groups to support this kind of thing. 

How do you engage Native American population into IT...for whatever reason.

## WebAssembly

### Keywords

* WebGl
* asm.js
* emscripten
* WebAssembly

### [Angry Bots](beta.unity3d.com/jonas/AngryBots/)

This game was created using asm.js (and also unity3d) which is just WebAssembly on steroids. 

### WebGL 

WebGL is OpenGL for the web. It's open-source, royalty-free and cross-platform. It uses low-level calls directly to the GPU. 

It's not for the faint of heart. 

WebGL support can be looked at by going to [CanIUse](caniuse.com/webgl) or checking [browser support](get.webgl.com).

### ASM.js and WebAssembly

ASM is not garbage collected or interpretted. It should be used for something that's CPU intensive, games, video processing and things of that nature. 

You can write code in any language if there is a transpiler that can take it down to highly optimized javscript. 

Enscripten is an LLVM based tool that takes C or C++ code and turns it into the javascript code mentioned above. Then this code can be run using asm.js which is a polyfill that can be pulled in. 

WebAssembly is expected to be an optimized, agreed upon standards-based implementation of ASM.js

Luke Wagner annouced WebAssembly on the mozilla blog and there is something up on [Github](github.com/WebAssembly). Basically, they want to deliver something that can be natively decoded and parsed and be done very quickly. 

If you compile asm.js "programs" into WebAssembly, the size can be reduced by about 60%. Most languages are going to be supported but for now it's only C/C++. JavaScript compilation to WebAssembly will also be supported at some point. 

WebAssembly is not supposed to replace JavaScript, it is designed to complement JavaScript. It will use compiled C++ apps (binary executables) and use Javascript as the glue. 

Brenden Eich, on his [website](brendeneich.com), has a video about ECMAScript Harmony and the rise of compilers. He talks about the ES versions and the cadence of releases. People are also using transpilers and compilers to get support for newer standards.

Check out DeadTrigger2 on Unity3D. It features MACHINE GUN CHICKEN SENTRIES!

## Innovation vs. Impatience

Courtesy of @codepo8

The deck talks mainly about JavaScript including the limitations of the language and the platform. 






