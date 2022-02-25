# PCB notes
## From Justin's notes:
"In this repository a second repo has been added as a submodule and is available in the libraries folder [here](./PCB/Library/kicad6-libraries/).  This is an example of storing all the symbols and footprints you collect and make over time in a single location.  Go and look at the source of this submodule [here](https://gitlab.com/r4space/kicad6-libraries.git).  

The advantage of this approach is that as you develop more PCBs you will collect and create an increasing number of custom symbols and footprints that are not provided in the std KiCAD libraries.  By adding this submodule to all of your projects you will always have access to this extended library.  The cost of this, however, is clearly that your project repos will get increasingly large as your personal library grows.  In the context of collaborative work in a company, this would not be a problem and the company likely has exactly such a custom in-house set of libraries and the repos are not released to a client with the entire submodule but rather a specific release repo is made for this.

For the project, this is an effective way of starting your own libraries repo and collaborating.

At any point, you are able to enter the folder containing this submodule and updating it via a normal git pull."
