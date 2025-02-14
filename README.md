# Free Whiteboard App

The **Whiteboard App** is an interactive, client‑side canvas built with HTML, CSS, and JavaScript. It allows you to create, move, and customize visual elements in real time—all with an intuitive drag‑and‑drop interface.

## Features

### Post-it Notes
- **Drag and Drop:**  
  Easily drag colorful Post-it notes from the dock onto the whiteboard canvas.
- **Dock Replacement:**  
  The right‑hand dock features four ready‑made Post-it notes (yellow, pink, blue, and green). When you drag one out, a new Post-it of the same color is automatically generated in its place.
- **Dynamic Positioning:**  
  Each used Post-it displays a **position pill** that updates in real time to show its relative position as percentages on the grid. The pill now shows **(0,0)** when a note is in the extreme lower‑left and **(100,100)** when in the extreme upper‑right.
- **Interactive Axes:**  
  When a Post-it is dragged over the x‑ or y‑axis, its background color changes and the position pill (and delete icon) temporarily hide to highlight the axis area.
- **Easy Deletion:**  
  A small **delete icon** (“×”) appears in the top left of each Post-it (except when over an axis) so you can remove notes with a click.

### Stickers
- **Sticker Functionality:**  
  In addition to Post-it notes, the dock now includes a sticker slot.
- **Numbered Stickers:**  
  The numbered sticker appears with a unique number. Dragging it from the dock onto the canvas reassigns it as a fully draggable element.
- **Auto-replacement:**  
  Once a numbered sticker is moved to the board, a new sticker with an incremented number is automatically generated in the dock.
- **Ranking Feature:**  
  If a red numbered sticker overlaps a Post-it note on the whiteboard, its number is used as a **ranking** value and will be included in the exported PDF table.
- **Always on Top:**  
  Stickers have a high z‑index, ensuring they remain visible above all Post-it notes and other elements.

### Background Customization
- **Upload Background:**  
  Replace the default grid by clicking the **Upload Background** button. Select an image file to personalize your whiteboard.

### Save as PNG
- **Capture Your Work:**  
  Click the **Save as PNG** button to capture the entire whiteboard—including Post-its, stickers, and your custom background—as a high‑quality PNG image.

### Export as PDF
- **Whiteboard Image Capture:**  
  The entire whiteboard (including background, Post-it notes, and stickers) is captured as an image and added to the top of the PDF.
- **Detailed Notes Table:**  
  Below the whiteboard image, a table is generated that lists all Post-it notes (excluding those still in the dock). For each note, the table displays:
  - The note text.
  - The **Pill X** and **Pill Y** values (i.e. the relative positions in percentages with bottom‑left as (0,0) and top‑right as (100,100)).
  - The note color.
  - The **Ranking** (if a red numbered sticker overlaps the note).
- **Interactive Data:**  
  This feature provides an easy-to-read summary of all the notes on your whiteboard.

### Enhanced Interactivity & Performance
- **Touch & Mouse Support:**  
  Enjoy smooth drag‑and‑drop interactions on both desktop and mobile devices.
- **Refactored Drag Manager:**  
  The code uses a centralized drag manager to optimize event handling, resulting in improved responsiveness and easier maintenance.

## Demo

![Whiteboard App Demo](screenshot.png)

Try it out [here](https://businessdatasolutions.github.io/whiteboard/)

## How to Use

1. **Clone the Repository.**

2. **Open the App:**

   Simply open the `index.html` file in your preferred web browser (Chrome, Firefox, etc.). The app runs entirely on the client side—no server setup is required.

3. **Using the App:**

   - **Post-it Notes:**  
     Drag a Post-it from the right‑hand dock onto the canvas. Click inside the Post-it to edit its content, and watch the position pill update automatically. To delete a Post-it, click the "×" icon.
     
   - **Stickers:**  
     Drag the numbered sticker from the dock onto the canvas. If a red numbered sticker overlaps a Post-it, its number is used as the note’s ranking. A new sticker will instantly replace the one you dragged.
     
   - **Axes & Grid:**  
     When a Post-it is moved over an axis, it changes color and the position pill (and delete icon) temporarily hide, emphasizing the axis.
     
   - **Upload Background:**  
     Click the **Upload Background** button, select an image file, and the whiteboard’s background will change from the grid to your chosen image.
     
   - **Save as PNG:**  
     Click the **Save as PNG** button to capture your whiteboard as a PNG image that you can download and share.
     
   - **Export as PDF:**  
     Click the **Export Notes PDF** button to generate a PDF. The PDF will display an image of your entire whiteboard at the top, followed by a table listing:
       - Note text.
       - Pill X and Pill Y values (relative positions).
       - Note color.
       - Ranking (if a red numbered sticker overlaps the note).

## Technologies Used

- **HTML5** for structure
- **CSS3** for styling (with Materialize CSS for a modern design)
- **Vanilla JavaScript** for interactivity
- **html2canvas** for capturing the whiteboard as a PNG image
- **jsPDF & AutoTable** for generating PDF exports

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! If you have ideas, improvements, or new features, please open an issue or submit a pull request.

## Acknowledgments

- [Materialize CSS](https://materializecss.com/) for the styling framework.
- [html2canvas](https://html2canvas.hertzen.com/) for enabling PNG export.
- [jsPDF & AutoTable](https://github.com/MrRio/jsPDF-AutoTable) for the PDF export functionality.