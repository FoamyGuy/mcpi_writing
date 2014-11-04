mcpi_writing
============
Module for use with mcpi to give access to writing characters with text made of blocks.

Demo Video: http://youtu.be/HoamEiueMe0

![mcpi_writing example](https://dl.dropboxusercontent.com/u/5724095/images/mcpi_writing_gh.png)

```python
from mcpi_writing import draw_str

mc = minecraft.Minecraft.create()
pos = mc.player.getPos()

# Draw a string
draw_str(pos.x, pos.y, pos.z - 1, "hello world")

# Specify foreground and background blocks
draw_str(pos.x, pos.y, pos.z - 1, "hello world", fg_block=57, bg_block=49)

# With border
draw_str(pos.x, pos.y, pos.z - 1, "hello world", border=True)

# With newlines
draw_str(pos.x, pos.y, pos.z - 1, "hello\nworld")

# facing north or south (currently no support for EAST/WEST)
NORTH = 2
SOUTH = 0
draw_str(pos.x, pos.y, pos.z - 1, "hello", facing=SOUTH)
draw_str(pos.x, pos.y, pos.z - 1, "hello", facing=NORTH)

```

I used Canarymod and RaspberryJuice, but theoretically it should work on the Raspberry Pi edition of MC too.

- http://canarymod.net/
- https://github.com/martinohanlon/CanaryRaspberryJuice

Music for youtube video:
https://soundcloud.com/thebrogrammer/cheese