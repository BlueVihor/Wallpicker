#!/bin/bash

# Set the directory containing wallpapers
WALLPAPER_DIR="$HOME/Wallpapers"

# Check if the wallpaper directory exists
if [ ! -d "$WALLPAPER_DIR" ]; then
    echo "Wallpaper directory not found: $WALLPAPER_DIR"
    exit 1
fi

# Let user pick wallpaper using rofi
SELECTED_WALLPAPER=$(find "$WALLPAPER_DIR" -type f \( -iname "*.jpg" -o -iname "*.png" -o -iname "*.jpeg" -o -iname "*.webp" \) | rofi -dmenu -p "Select Wallpaper")

# Exit if no selection made
[ -z "$SELECTED_WALLPAPER" ] && exit 0

feh --bg-scale $SELECTED_WALLPAPER

