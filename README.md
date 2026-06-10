# -2D-Graphics-Editor
2D Graphics Editor in C

Overview

This project is a menu-driven 2D Graphics Editor implemented in C using a 2D character array as the drawing canvas. The canvas is initially filled with the underscore character ("_"), while graphical objects are drawn using the asterisk character ("*").

The editor allows users to create, modify, delete, and display basic geometric shapes directly in the console.

Features

- Draw graphical objects:
  - Line
  - Rectangle
  - Circle
  - Triangle
- Add multiple shapes to the canvas
- Delete shapes using unique Shape IDs
- Modify existing shapes
- Display the current canvas
- List all active shapes
- Uses classic computer graphics algorithms:
  - Bresenham's Line Drawing Algorithm
  - Midpoint Circle Algorithm

Data Structures Used

Shape Structure

Each shape is stored with:

- Unique ID
- Shape type
- Coordinates
- Radius (for circles)
- Active/Deleted status

Canvas

A 2D character array:

char canvas[HEIGHT][WIDTH];

Canvas Size:

- Width = 60
- Height = 30

Supported Shapes

1. Line

Input:

x1 y1 x2 y2

2. Rectangle

Input:

Top-Left (x1, y1)
Bottom-Right (x2, y2)

3. Circle

Input:

Center (x, y)
Radius r

4. Triangle

Input:

(x1, y1)
(x2, y2)
(x3, y3)

Menu Options

=== 2D Graphics Editor ===
1. Add Shape
2. Delete Shape
3. Modify Shape
4. Display Canvas
5. List Active Shapes (IDs)
6. Exit

Algorithms Used

Bresenham's Line Algorithm

Used for drawing:

- Lines
- Rectangle edges
- Triangle edges

Advantages:

- Efficient
- Uses integer arithmetic
- Fast rendering

Midpoint Circle Algorithm

Used for drawing circles.

Advantages:

- Symmetric plotting
- Efficient circle generation
- Uses integer calculations

Compilation

GCC

gcc graphics_editor.c -o graphics_editor

Running the Program

./graphics_editor

Windows

graphics_editor.exe

Example Workflow

1. Add a rectangle.
2. Add a circle.
3. Display canvas.
4. Modify the circle.
5. Delete the rectangle.
6. Display updated canvas.

Project Structure

graphics_editor.c
README.md

Learning Outcomes

This project helps understand:

- 2D Graphics Fundamentals
- Computer Graphics Algorithms
- Structures in C
- Arrays and Memory Management
- Menu-Driven Programming
- Shape Rendering Techniques

Future Improvements

- Shape filling
- Color support using ANSI escape codes
- Save and load drawings from files
- Undo/Redo functionality
- Shape movement using keyboard controls
- Scaling and rotation transformations
- GUI implementation using graphics libraries

Author

Shivam Vishwakarma

License

This project is developed for educational and learning purposes.
