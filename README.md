# OneLoneCoffeeEngine
A Java Translation of the OneLoneCoder GameEngine, originally made by Javidx9

(The OneLoneCoffee game engine was made by CasuallyCritical)

USAGE:

I don't care what you do with this Engine, but please give credit for the engine! I would be happy if you did.

GUIDE:

The library is simple to use.

When you are setting up:

1) Create a main class
2) Main class MUST EXTEND GameEngine

When you are ready

1) In your main function, create a new GameEngine that calls back your main class.
2) call "constructWindow" to create a JFrame
3) call "constructGraphics" to create a BufferedImage (this will be what you use to draw to the canvas)
4) call "start" on the GameEngine

You should Override OnUserCreate and OnUserUpdate as well, so you can Add what you need

OnUserUpdate is your Update function, it should pass a float for the delta time.

DRAW Functions:

Draw(int color, int x, int y) <- creates a pixel at x, y coordinates with the color requested

DrawFill(int color, int x, int y, int w, int h) <- creates a box of Width w by Height h at x, y coordiantes with the color requested.

DrawSprite(Sprite sprite, int x, int y, int w, int h) <- creates a sprite using the passed values

SPRITES:

Sprites are fairly simple, pass a File in the resources folder of your project and it will create one off that, OR you can make a blank one by passing the Width and Height you require
