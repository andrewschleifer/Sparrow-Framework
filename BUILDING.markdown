Sparrow: Tips for building an app
=================================

A First look at Sparrow
-----------------------

In the folder 'samples/demo', you will find an Xcode project that shows the most basic Sparrow
features and how to use them. Just open the project in Xcode, compile and run - everything should
work out of the box.

Creating a new Xcode project that uses Sparrow
----------------------------------------------

In the folder 'samples/scaffold', you will find an Xcode project that contains a bare-bone Sparrow
application. We recommend that you use this project as a starting point for your game. Please follow
this steps to use this Scaffold:

### Preconditions: ###

Sparrow is linked to your application via Xcode project references. This has the advantage that it's
easy to update Sparrow (just download a new release and overwrite the old one in the same directory)
and that you can easily step into Sparrow source code, in case you want to do so.

### This has to be done only once: ###

1. Set up a shared build output directory that will be shared by all Xcode projects.
   * In the Xcode preferences, tab: "Building", set "Place Build Products in" to 
    "Customized location" and specify a common build directory (anywhere you want).
   * Set "Place Intermediate Build Files in" to "With build products."
2. Add a "Source Tree" variable that Xcode can use to dynamically find Sparrow.
   * In the Xcode preferences, tab: "Source Trees", create a new Source Tree variable.
   * For Sparrow, create SPARROW_SRC and let it point to /some_valid_path/sparrow/src/

### Creating your new project: ###

1. Copy the "scaffold"-folder to the place where you want to have your game project.
2. Open "AppScaffold.xcodeproj"
3. Build and run - just to see if everything works fine. If it does not work, check if you have 
   created the SPARROW_SRC variable in Xcode, and if it points to the right place.
4. In Xcodes menu, click on "Project" -> "Rename ..."
5. Enter the name of your game.
6. That's it! Now you can start to develop your game with Sparrow. 

### Selecting target hardware: iPhone / iPod Touch / iPad ###

1. Enter the project Settings, tab: "Build"
2. Select the target of your choice for the setting "Targeted Device Family"

That's it!