# Asciin.py

![logo](https://raw.githubusercontent.com/Rickaym/Asciin.py/main/assets/inverted_logo.png)

A 2D and 3D Ascii game engine written for performance (still under development)

Current docs: **https://asciinpy.readthedocs.io/en/latest/**
pypi project: **https://pypi.org/project/Asciin.py/**

### Status Demo

1. **Matrixes Patterns**
   <br> An example in working with PixelPainters.

![demo](https://raw.githubusercontent.com/Rickaym/Asciin.py/main/assets/LuckyDevStuff_render.gif)

More examples [here](https://github.com/Rickaym/Asciin.py/tree/main/examples/).

### Installing

**Python 2.7 or higher is required**

```js
// Windows
py -m pip install -U asciin.py

// Linux/macOS
python -m pip install -U asciin.py
```

### Simple Example

```py
from Asciinpy import Square, Displayable, Window, Resolutions

# Define a window
window = Window(resolution=Resolutions._60c)

@window.loop()
def game_loop(screen):
   # type: (Displayable) -> None
   coordinate = (0, 0)
   length = 8
   texture = "%"
   Square = Square(coordinate, length, texture)
   while True:
      screen.blit(Square)
      screen.refresh()

window.run()
```

Contact me at Neo#1844 for inquiries.
