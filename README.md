mcpi_writing
============
Module for use with mcpi to give access to writing characters with text made of blocks.

![mcpi_writing example](https://dl.dropboxusercontent.com/u/5724095/images/mc_py_writing1.PNG)

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
```

Music for youtube video:
https://soundcloud.com/thebrogrammer/cheese