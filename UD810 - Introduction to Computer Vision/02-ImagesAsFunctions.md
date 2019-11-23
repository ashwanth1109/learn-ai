# IMAGES AS FUNCTIONS

A 2D image can be represented as a function I(x,y). Computer Vision is about taking these functions and computing something from them (e.g. compute an image from an original image).

An image represented as f(x,y) where x ranges from a to b, and y ranges from c to d which corresponds to an Intensity value for a given x and y value. Intensity values range from a min and max value as derived from the range of x and y values.

```
f:x(a to b), y(c to d) => I[min,max]
```

Given that this function maps from two variables (x and y) to one intensity value (I), the function goes from R^2 to R. The min represents the darkest shade of black in the image and max represents the lightest shade of white in the image for a grayscale image.

### Color Images

Color images can also be represented as functions in the form of a "vector-valued" function.

```
f(x,y) = [r(x,y)]
         [g(x,y)]
         [b(x,y)]
```

### Digital Images

When you work with digital images, you need to:

- Sample the 2D space on a regular grid
- Quantize each sample (to the nearest integer)

So, if you quantize each sample to 8 bits, then the value will range from 0 to 255.
