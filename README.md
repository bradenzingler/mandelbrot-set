# mandelbrot-set

A visualizer for the Mandelbrot Set.

![colorful_mandelbrot](https://github.com/bradenzingler/mandelbrot-set/assets/124199084/18909bbb-7b45-41f0-b753-c8b2aab67c54)


## How to use
Clone the repo and run the ```Mandelbrot.java``` file. To configure colors and other parameters, see the function ```getIterationColor()```.


## How it works
The [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set) is a set that contains complex numbers that do not diverge when iterated over the function f(z) = z^2 + c.
The set is drawn by iterating over each pixel and calculating the iteration for the point. The iteration is then used to determine the color of the pixel.
The color can be adjusted to show the divergence of the point. Below is an example where high divergence is assigned darker values.

![image](https://github.com/bradenzingler/mandelbrot-set/assets/124199084/f5f63f3b-8bc9-4fdf-94a7-b1268b45fc8e)

## Playing with colors
What if we make the color a function of the iteration number?

Here is a pretty cool example: ```Color color = new Color(iteration % 255, iteration % 255, iteration % 255);```
It doesn't look a lot different, but you can see there is a slight gradient between the transition from light to dark pixels.

![image](https://github.com/bradenzingler/mandelbrot-set/assets/124199084/1830c552-2fe0-4cb7-b255-61add821fbb5)



