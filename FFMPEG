#!/bin/bash

resolutions=(1920 1024 320 100)

originalHeight=1800
originalWidth=4320

for res in "${resolutions[@]}"; do
    height=$((originalHeight * res / originalWidth))
    ffmpeg -i desktop.png -vf "scale=$res:$height" "./momo/desktop_${res}.webp"
done
