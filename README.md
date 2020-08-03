## lunasvg
lunsvg is a standalone c++ library to create, animate, manipulate and render SVG files.

![svg2png generated PNG](/example/tiger.svg.png)

## example
```cpp
#include <lunasvg/svgdocument.h>

using namespace lunasvg;

int main()
{
    SVGDocument document;
    document.loadFromFile("tiger.svg");
    
    Bitmap bitmap = document.renderToBitmap();
    
    // do something useful with the bitmap.
    
    return 0;
}

```

## features
- Basic Shapes : rect, circle, ellipse, line, polyline, polygon, path.
- Paint server : solidColor, linearGradient, radialGradient, pattern.
- Clipping, Masking and Compositing : clipPath, mask, group opacity.
- Document Structure: defs, svg, g, use, symbol.
- Coordinate Systems, Transformations and Units.

## build
- Install [cmake](https://cmake.org/download/) if not already installed.

Create a build directory.
```
mkdir build
```
Run cmake command inside build directory.
```
cd build
cmake ..

```
Run make to build lunasvg.

```
make -j 2
```
To install lunasvg library.

```
make install
```

## demo
While building lunasvg library it generates a simple SVG to PNG converter which can be used to convert SVG file to PNG file.

Run Demo.
```
svg2png [filename] [resolution] [bgColor]
```

## support
<a href="https://www.buymeacoffee.com/sammycage" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;" ></a>
