# Shape Viewer

A web-based application designed to visualize and manipulate 2D shapes. This project demonstrates advanced web development techniques, including file parsing, dynamic shape rendering, and interactive user interfaces. It serves as both a practical tool for viewing geometric shapes and a showcase of front-end development skills.

## How to Run and Test the Code

1. Clone this repository to your local machine.
2. Open the `index.html` file in a modern web browser (Chrome, Firefox, Safari, or Edge recommended).
3. To test with a shape file:
   - Click the "Choose File" button and select a .txt or .rtf file with shape definitions.
   - Alternatively, click the "Use Sample File" button to load a predefined set of shapes.
4. Shapes should render in the viewport. You can drag shapes to move them and use the blue handle above each shape to rotate it.

## Test Input Files

Sample shape files for testing are located in the `samples` directory of this repository:

- `sample.txt.rtf`: Basic shapes including rectangles
- `samplePolygon.txt.rtf`: Includes polygon shapes
- `sampleTriangle.txt.rtf`: Includes triangle shapes
- `test_shapes.txt`: A comprehensive test file with various shapes

## Additional Information

### Completed Assignment Iterations

All four iterations of the assignment have been completed:

1. User Interface Layout
2. Shape File
3. Shape Rendering
4. Polygon Support

### Implemented Bonus Features

The following bonus features have been implemented:

1. Shape Translation (drag-and-drop functionality)
2. Shape Rotation
3. Extra Feature: "Use Sample File" button for quick testing without file upload

### Known Problems

There are no major known problems with the solution. However:

- Performance with very large numbers of shapes (approaching 100,000) has not been extensively tested.
- The "Save as" functionality for saving modified shapes has not been implemented.

## Shape File Format

Each line in the shape file should define a shape using the following format:

- **Rectangle**: `Rectangle, x, y, z, width, height, color`
- **Triangle**: `Triangle, x1, y1, x2, y2, x3, y3, z, color`
- **Polygon**: `Polygon, x1, y1, x2, y2, ..., xn, yn, z, color`

**Parameters:**
- **x, y**: Coordinates
- **z**: Z-index for layering
- **width, height**: Dimensions for rectangles
- **color**: 6-digit hexadecimal color code

---

## Development Process

### Initial Setup
- Created a basic HTML structure with a file input and viewport.

### File Parsing
- Implemented RTF stripping and shape parsing from the input file.

### Shape Rendering
- Developed functions to render rectangles, triangles, and polygons.

### Interactivity
- Added drag-and-drop functionality for shapes.
- Implemented shape rotation using a blue handle above each shape.

### Error Handling
- Integrated robust error handling and debugging output.

---

## Hosting and CI/CD

- **Platform**: Azure Static Web Apps
- **Automation**: GitHub Actions for CI/CD
- **Workflow**: YAML-defined pipeline for automated build and deployment
- **URLs**: 
  - [Azure App Link](https://proud-island-0100d7510.5.azurestaticapps.net/)
  - [Custom Domain](https://shapeviewer.com) (DNS propagation may take time)

---

## Challenges Faced and Solutions Implemented

### RTF Formatting
- **Challenge**: RTF formatting interfered with shape parsing.
- **Solution**: Implemented a robust RTF stripping function using regular expressions.

### Shape Rendering
- **Challenge**: Difficulty rendering complex shapes like triangles and polygons.
- **Solution**: Utilized HTML5 Canvas for accurate representation.

### Drag and Drop
- **Challenge**: Implementing smooth drag-and-drop while maintaining shape integrity.
- **Solution**: Developed a real-time updating system to keep shapes within the viewport.

### Shape Rotation
- **Challenge**: Adding rotation capability without affecting other shape properties.
- **Solution**: Implemented rotation using CSS transforms, preserving original positions and sizes.

### Error Handling
- **Challenge**: Gracefully handling various errors without crashing the application.
- **Solution**: Integrated a centralized error handling system.

### Performance
- **Challenge**: Maintaining responsiveness with multiple shapes.
- **Solution**: Optimized rendering functions and used efficient data structures.

---

## Known Limitations

- **Performance**: May degrade with a very large number of shapes.
- **Input**: Limited to static file input (no real-time shape creation).

---

## Future Improvements

- **Navigation**: Add zoom and pan functionality.
- **Shape Creation**: Implement a user interface for creating new shapes directly.
- **Persistence**: Add save/load functionality for shape configurations.
- **Optimization**: Enhance performance to handle up to 100,000 shapes.

---

## How to Run and Test the Code

1. **Run**: 
   - Open `ShapeViewer.html` in your web browser, or
   - Access the live demo via the provided Azure or custom domain links.
2. **Test**: 
   - Use the provided sample shape files in the `samples` directory of the GitHub repository.
   - Click the "Use Sample File" button to load a predefined sample file.

---
