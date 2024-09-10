# Shape Viewer

A web-based application for viewing and manipulating 2D shapes.

## Features

- Load and render shapes from custom text files
- Support for rectangles, triangles, and polygons
- Drag-and-drop functionality for moving shapes
- Rotation of shapes
- Error handling for invalid shape definitions

## How to Use

1. Open ShapeViewer.html in a web browser
2. Click "Choose File" to select a shape file
3. Shapes will be rendered in the viewport
4. Drag shapes to move them
5. Use the blue handle above each shape to rotate it

## Shape File Format

Each line in the shape file should define a shape using the following format:

- Rectangle: `Rectangle, x, y, z, width, height, color`
- Triangle: `Triangle, x1, y1, x2, y2, x3, y3, z, color`
- Polygon: `Polygon, x1, y1, x2, y2, ..., xn, yn, z, color`

Where:
- x, y: coordinates
- z: z-index for layering
- width, height: dimensions for rectangles
- color: 6-digit hexadecimal color code

## Known Limitations

- Performance may degrade with a very large number of shapes
- Limited to static file input (no real-time shape creation)

## Future Improvements

- Add zoom and pan functionality
- Implement shape creation interface
- Add save/load functionality for shape configurations

## Development

This project was developed as part of a programming assignment. It demonstrates skills in HTML, CSS, JavaScript, and handling of complex user interactions in a web environment.



Brief report on the development process, challenges faced, and solutions implemented:
Development Process:

Initial Setup: Created a basic HTML structure with a file input and viewport.
File Parsing: Implemented RTF stripping and shape parsing from the input file.
Shape Rendering: Developed functions to render rectangles, triangles, and polygons.
Interactivity: Added drag-and-drop functionality for shapes.
Advanced Features: Implemented shape rotation.
Error Handling: Integrated robust error handling and debugging output.

Challenges Faced and Solutions Implemented:

RTF Formatting:
Challenge: Input files contained RTF formatting that interfered with shape parsing.
Solution: Implemented a robust RTF stripping function using regular expressions.
Shape Rendering:
Challenge: Rendering complex shapes like triangles and polygons.
Solution: Utilized HTML5 Canvas for drawing non-rectangular shapes, ensuring accurate representation.
Drag and Drop:
Challenge: Implementing smooth drag-and-drop while maintaining shape integrity.
Solution: Created a dragging system that updates shape positions in real-time and ensures shapes stay within the viewport.
Shape Rotation:
Challenge: Adding rotation capability without affecting other shape properties.
Solution: Implemented a rotation handle and used CSS transforms to rotate shapes, preserving their original position and size.
Error Handling:
Challenge: Gracefully handling various types of errors without crashing the application.
Solution: Implemented a centralized error handling system that displays errors to the user and logs them to the console.
Performance:
Challenge: Ensuring the application remains responsive with multiple shapes.
Solution: Optimized rendering functions and used efficient data structures for shape management.

Future Improvements:

Implement zooming and panning for better navigation of complex shape arrangements.
Add a user interface for creating new shapes directly in the viewer.
Implement save and load functionality for shape configurations.
Optimize for handling a very large number of shapes (up to 100,000).