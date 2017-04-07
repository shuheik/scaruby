# Scaruby

Scaruby is a Ruby-like lightweight scripting library for Scala.  Scaruby is not a thin layer of `java.io`
but a thick layer.  Users don't need to know the detail of `java.io`.

## Usage

Now Scaruby supports Scala 2.11.X and Scala 2.12.X.

Add the following lines to your build.sbt:

```scala
resolvers += "Sonatype OSS Snapshots" at "https://oss.sonatype.org/content/repositories/snapshots"

libraryDependency += "com.github.scaruby" %% "scaruby" % "0.1-SNAPSHOT"
```

and you can use Scaruby like the following after importing the package `com.github.scaruby.scaruby._`:

```scala
import com.github.scaruby.scaruby._

val content = SFile.readAllStrings("file.txt")
```
