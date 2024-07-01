Structure of Shared Libraries

PROJECT ROOT
+- src/
|   +- org/
|       +- yourorg/
|           +- TimeUtils.groovy
+- vars/
|   +- helloWorld.groovy
+- resources/
|   +- exampleResource.txt
+- test/
|   +- org/
|       +- yourorg/
|           +- TimeUtilsTest.groovy
+- README.md
+- build.gradle (or pom.xml if using Maven)

src, vars, resources, test are the main components in the shared libraries.

src -> holds the main code for your shared library.
vars -> contains simpler scripts that define global functions or variables you can call directly in your Jenkins pipeline.
resources -> holds additional files your library might need. Resource files like configuration files, templates, or text files.
test -> contains tests to verify that your shared library code works correctly.

Purpose of Each Directory
src: Where your core reusable code lives. Think of it as the main toolbox.
vars: For simple, easily accessible tools or functions you frequently use in pipelines.
resources: Extra files that your tools might need to work properly.
test: Where you check that your tools are working correctly before using them in your actual pipelines.


