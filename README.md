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