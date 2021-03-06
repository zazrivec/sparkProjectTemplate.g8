# Spark Project Template
A [Giter8][g8] template for Scala Spark Projects.

## What this gives you

This is a fork of [Holden Karau's Spark Project Template](https://github.com/holdenk/sparkProjectTemplate.g8), with my own choice of different plugins and UT style. Check out her repo for the latest version of the real thing. 

This template will bootstrap a new spark project with everyone's "favourite" wordcount example (modified for stop words). You can then replace the wordcount example as desired, and customize the Spark components your project needs.


To encourage good software development practice, this starts with a project at 100% code coverage (e.g. one test :p), while its expected for this to decrease, we hope you use the provided [spark-testing-base][stb] library or similar option.

A basic release process with auto-incrementing version is in place in the build script, based on sbt-git and sbt-release and heavily inspired [from those very useful sbt release tips from Jean Helou](http://blog.byjean.eu/2015/07/10/painless-release-with-sbt.html).

## Creating a new project from this template

Have g8 installed? You can run it with:

```bash
g8 sv3nd/sparkProjectTemplate --name=projectname --organization=com.my.org --sparkVersion=2.2.0
```

Using sbt (0.13.13+)? just do

```bash
sbt new sv3nd/sparkProjectTemplate.g8
```

And specify values when prompted for the template variables.

The version of the project is handled by the [sbt-git](https://github.com/sbt/sbt-git) plugin, so it's expecting you to `git init` the project as soon as it's created.

See also the [README.md](src/main/g8/README.md) on the generated project for more instructions on how to build and release it. 

## Related

Want to build your application using the Spark Job Server? The [spark-jobserver.g8][sjsg8] template can help you get started too.

## License

This project is available under your choice of Apache 2 or CC0 1.0.
See <https://www.apache.org/licenses/LICENSE-2.0> or <https://creativecommons.org/publicdomain/zero/1.0/> respectively.
This template is distributed without any warranty.

[g8]: http://www.foundweekends.org/giter8/
[stb]: https://github.com/holdenk/spark-testing-base
[sjsg8]: https://github.com/spark-jobserver/spark-jobserver.g8
