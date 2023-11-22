# CAIRO-codes
Certainly! To run Cairo code, you typically need to use a programming language that supports Cairo graphics. Below is a simple example using Python and the Pycairo library to draw a red rectangle:

```python
import cairo

width, height = 400, 300

surface = cairo.ImageSurface(cairo.FORMAT_ARGB32, width, height)
context = cairo.Context(surface)

# Set background color
context.set_source_rgb(1, 1, 1)  # White
context.paint()

# Draw a red rectangle
context.set_source_rgb(1, 0, 0)  # Red
context.rectangle(50, 50, 200, 100)
context.fill()

# Save the result to a PNG file
surface.write_to_png('cairo_example.png')
```

Make sure you have the Pycairo library installed (`pip install pycairo`), and then you can run this script. It creates a white background and draws a red rectangle on it. The result will be saved as "cairo_example.png" in the same directory.

Note: Running graphics code may require additional setup depending on your environment, and this example assumes you have the necessary libraries installed.
