# Inform 6 Playground

_Simplified Distribution of the Inform 6 Interactive Fiction System_

This repository contains a simplified distribution of [Inform 6](https://www.inform-fiction.org/). This includes the standard library as well as the executables for Mac and Windows systems.

The Inform 6 library is currently distributed at [inform6lib](https://gitlab.com/DavidGriffith/inform6lib). This repository includes version 6.12.6 of the library.

The Inform 6 source is currently distributed at [Inform6](https://github.com/DavidKinder/Inform6). This repository includes version 6.41 of Inform.

Beyond being distributed at the above links, all of the Inform 6 ecosystem is available within the ["inform6"](https://ifarchive.org/indexes/if-archive/infocom/compilers/inform6/) area of the if-archive.

## Usage

If you clone this repository, it's set up to ignore a `project` or `projects` directory. You can set the location of the provided Inform 6 executable on your system path. A simple Inform 6 example would be this:

```inform6
[ Main;
  print "Testing Inform 6^";
];
```

If that code is stored in a file called `learn.inf`, then you could then compile that with:

`inform6 learn.inf`

Let's say that you have a program that uses the Inform 6 library. Consider this:

```inform6
Constant Story "RUINS";
Constant Headline "^An Interactive Example^";

Include "Parser";
Include "VerbLib";

[ Initialise;
  "^^^A discovery looms before you ...";
];

Include "Grammar";
```

If that code is stored in a file called `ruins.inf`, then you could compile that with:

`inform6 ruins.inf +include_path=../lib/`

With Inform 6, you can also provide what are called "ICL commands" within the source code of your program. If you didn't want to specify the include path at the command line, as above, you could include this line in your source at the top of the file:

```inform6
!% +include_path=../lib
```

Keep in mind that if you place your project in a subdirectory within your projects directory, you will have to adjust the relative paths accordingly. The idea, however, is that everything is done relative to the Inform 6 playground structure.
