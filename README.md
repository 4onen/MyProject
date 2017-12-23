#Dad's quick CMake tutorial

In the root of this project, create a folder called "MyBuild". (You might notice this directory was added to the .gitignore. 

###Using the CMake GUI
Select the root directory of the project as the "Source" directory and "MyBuild" as the "Build" directory. Click configure. Wait for CMake to perform its computation, then hit Generate. This should create a Visual Studio .sln in the MyBuild directory. Open this solution in Visual Studio and hit F7 to verify it builds without errors. To build any of the executables, right click on the Visual Studio project with the same name (under the Solution Expolorer), then click "Set as startup project" in the context menu. Build the project with F7 (clicking Reload if prompted) and press Ctrl+F5 to debug. Voila! Output.

###Using the CMake CLI
Navigate to the MyBuild directory you created in this project folder. There, run the command `cmake ..`, which will tell CMake to run with the directory above this as the source directory. CMake will generate makefiles or a visual studio project (platform dependent) into the MyBuild directory. If it makes makefiles, I'm sure future me can figure out what to do with them. If it makes Visual Studio project files, follow the same build steps as using the CMake GUI.



That should about cover everything! Great job!
