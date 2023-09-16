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

If that code is stored in a file called `learn.t`, then you could then compile that with: `inform6 learn.t`.
