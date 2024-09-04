# Shape Viewer

Shape Viewer is a web-based application that allows users to upload and visualize 2D shapes from a custom file format.

## Features

- Upload shape files (.txt, .shapefile, or .rtf)
- Display shapes on a canvas
- Support for multiple shape types (currently rectangles)
- Color rendering of shapes

## How to Use

1. Clone the repository or download the ShapeViewer.html file.
2. Open ShapeViewer.html in a web browser.
3. Click on "Choose File" and select a shape file.
4. The shapes from the file will be displayed in the viewport.

## Shape File Format

The shape file should contain one shape per line in the following format:

```
ShapeType, X, Y, Z-index, Width, Height, Color
```

Example:
```
Rectangle, 0, 0, 0, 50, 50, ff0000
```

This creates a red square at coordinates (0,0) with width and height of 50 pixels.

## Future Improvements

- Add support for more shape types (circles, triangles, etc.)
- Implement zoom and pan functionality
- Add ability to edit shapes interactively
- Implement save functionality to export modified shapes

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
