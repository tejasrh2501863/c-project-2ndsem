Features
Draw Lines
Draw Rectangles
Draw Circles
Draw Triangles
Add, Modify, and Delete Objects
List All Objects
Render Shapes on an ASCII Canvas
Menu-Driven Interface
Lightweight and Portable
Canvas Specifications
Property	Value
Width	80
Height	24
Drawing Character	*
Background Character	_
Supported Shapes
Line
Defined by two endpoints:

(x1, y1) -> (x2, y2)
Rectangle
Defined by top-left and bottom-right coordinates:

(x1, y1) --------
|               |
|               |
-------- (x2, y2)
Circle
Defined by center coordinates and radius:

Center: (x, y)
Radius: r
Triangle
Defined by three vertices:

(x1, y1)
(x2, y2)
(x3, y3)
Algorithms Used
Bresenham's Line Algorithm
Used for efficient line rendering using integer arithmetic.

Midpoint Circle Algorithm
Used for drawing circles using symmetry and incremental calculations.

Project Structure
.
├── graphics_editor.c
└── README.md
Compilation
Compile using GCC:

gcc graphics_editor.c -o graphics_editor -lm
Running the Program
./graphics_editor
Menu
1. Add object
2. Delete object
3. Modify object
4. Display picture
5. List objects
0. Exit
Example Usage
Add a Rectangle
Enter choice: 1

Choose shape type:
1. Line
2. Rectangle
3. Circle
4. Triangle

Enter shape type: 2
Enter top-left x y and bottom-right x y:
10 5 25 15
Display Canvas
Enter choice: 4
Example Output:

__________****************
__________*______________*
__________*______________*
__________*______________*
__________****************
Data Structure
struct shape {
    int kind;
    int ax, ay;
    int bx, by;
    int cx, cy;
    int r;
};
Supported shape types:

Kind	Shape
1	Line
2	Rectangle
3	Circle
4	Triangle
Maximum number of objects:

#define MAX 100
Limitations
Maximum of 100 objects
Fixed canvas size (80 × 24)
No save/load functionality
No color support
Outline-only shapes
Limited input validation
Future Enhancements
Filled Shapes
Polygon Support
Undo/Redo Functionality
Save and Load Drawings
Dynamic Canvas Resizing
Shape Translation and Scaling
Colored Terminal Rendering
Image Export Support
Learning Outcomes
This project demonstrates:

C Programming Fundamentals
Structures and Arrays
Menu-Driven Applications
ASCII Graphics Rendering
Bresenham's Line Algorithm
Midpoint Circle Algorithm
Basic Graphics Pipeline Concepts
License
This project is licensed under the MIT License.

Author
Developed as a simple educational project to explore computer graphics concepts using the C programming language.

⭐ If you like this project, consider giving it a star on GitHub!

About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Releases
No releases published
Create a new release
Packages
No packages published
Publish your first package
Contributors
1
@shreyasgdurs-collab
shreyasgdurs-collab
Languages
C
100.0%
Suggested workflows
Based on your tech stack
CMake based, multi-platform projects logo
CMake based, multi-platform projects
Build and test a CMake based project on multiple platforms.
MSBuild based projects logo
MSBuild based projects
Build a MSBuild based project.
CMake based, single-platform projects logo
CMake based, single-platform projects
Build and test a CMake based project on a single-platform.
More workflows
Footer
