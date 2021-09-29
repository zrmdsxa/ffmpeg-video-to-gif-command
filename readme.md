ffmpeg -y -i %1 -vf palettegen palette.png

ffmpeg -y -i %1 -i palette.png -lavfi paletteuse %1.gif
