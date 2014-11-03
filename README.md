mcpi_writing
============
Module for use with mcpi to give access to writing characters with text made of blocks.

```
mc = minecraft.Minecraft.create()
pos = mc.player.getPos()

# Draw a string
draw_str(pos.x, pos.y, pos.z - 1, "hello world")

# Speficy foreground and background blocks
draw_str(pos.x, pos.y, pos.z - 1, "hello world", fg_block=57, bg_block=49)
```

Music for youtube video:
https://soundcloud.com/thebrogrammer/cheese