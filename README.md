# 🧶 Knitting Pattern Counter

A web-based tool that automatically analyzes knitting pattern images and overlays stitch numbers to help you follow along while knitting.

## Features

- **Automatic Grid Detection**: Upload an image and the grid is automatically detected and processed
- **Individual Stitch Numbering**: Each cell shows its position in consecutive color sequences (1, 2, 3...)
- **Real-time Adjustments**: Fine-tune grid alignment with X/Y offsets and grid size controls
- **Color Grouping**: Adjustable color tolerance to group similar shades together
- **Visual Overlays**: Toggle grid lines and numbering displays
- **Pattern Analysis**: Detailed breakdown showing rows, columns, total stitches, and colors used
- **Download Functionality**: Save your numbered pattern as a PNG image
- **Color Legend**: Visual reference for all colors detected in the pattern

## How to Use

1. **Upload Image**: Drag and drop or click to select your knitting pattern image
2. **Automatic Processing**: The app automatically detects the grid and processes the pattern
3. **Fine-tune Settings** (if needed):
   - Adjust **Grid Size** if the detection isn't perfect
   - Use **X/Y Offsets** to align the grid with your pattern
   - Increase **Color Tolerance** to group similar colors together
   - Toggle **Show All Numbers** to see both cell numbers and consecutive counts
   - Toggle **Show Grid Overlay** to show/hide grid lines
4. **Customize**: Click 🎨 **Change Grid Color** to find a color that contrasts well with your pattern
5. **Download**: Click 💾 **Download Image** to save your numbered pattern

## Controls

| Control | Description |
|---------|-------------|
| **Auto Detect Grid** | Manually trigger grid detection (runs automatically on upload) |
| **Grid Size** | Size of each grid cell in pixels |
| **X Offset** | Horizontal offset to align grid with pattern |
| **Y Offset** | Vertical offset to align grid with pattern |
| **Color Tolerance** | How similar colors need to be to group together (higher = more grouping) |
| **Show All Numbers** | Toggle between showing all info vs just consecutive counts |
| **Show Grid Overlay** | Show/hide the grid lines |
| **Change Grid Color** | Randomize grid color for better visibility |
| **Download Image** | Save the numbered pattern as PNG |

## Pattern Information

The app displays:
- **Rows**: Number of pattern rows
- **Columns**: Number of pattern columns
- **Total Stitches**: Total number of individual stitches
- **Colors Used**: Number of different colors detected
- **Pattern Breakdown**: Row-by-row color sequence (A3, B2, A1 format)
- **Color Legend**: Visual reference showing color samples with symbols

## Numbering System

- **Top number**: Overall stitch number (1, 2, 3, 4...)
- **Bottom number**: Position within consecutive color sequence (1, 2, 3, then resets to 1 for new color)
- When "Show All Numbers" is disabled, only consecutive positions are shown

## Supported Formats

- JPG, PNG, GIF images
- Works best with clear grid patterns
- Knitting charts with distinct color regions

## Tips for Best Results

1. Use high-contrast knitting charts for better color detection
2. Increase Color Tolerance (50-90) if similar colors aren't being grouped
3. Adjust offsets if the pattern has borders or headers
4. Use "Change Grid Color" to find one that contrasts with your pattern background
5. Download the processed image to reference while knitting

## Technical Details

- Pure HTML/CSS/JavaScript - no server required
- Works entirely in your browser
- Uses HTML5 Canvas for image processing
- Automatic grid detection using edge detection algorithms
- Real-time updates when adjusting settings

---

Simply open `index.html` in your web browser to start using the tool!