# Whiteboard App

This is a simple, interactive whiteboard application built with plain HTML, CSS, and JavaScript. The app allows users to:

- **Drag and drop** Post-it notes onto the whiteboard canvas.
- Use a **dock** on the right side of the canvas that contains four ready-made Post-its (yellow, pink, blue, and green). When a Post-it is dragged from the dock into the canvas, a replacement of the same color is automatically created in the dock, preserving the dock order.
- **Edit** the content of each Post-it.
- See a small **position pill** (displaying the relative position in percentages) that is automatically positioned at the bottom left of each used Post-it.
- Remove a Post-it by clicking a small **delete icon** in the top left corner (the delete icon is hidden when the Post-it touches an axis).
- **Upload a background image** to replace the default grid.
- **Save the whiteboard** as a PNG image.

## Demo

![Whiteboard App Demo](screenshot.png)

Try it out ![here](https://businessdatasolutions.github.io/whiteboard/)

## How to Use

1. **Clone the repository:**

2. **Open the app:**

   Open the `index.html` file in your favorite web browser (Chrome, Firefox, etc.). No server is required as the app is entirely client-side.

3. **Using the App:**

   - **Dock & Drag Post-its:**  
     On the right-hand side, you will see the dock with four Post-its in different colors. Click and drag a Post-it from the dock onto the canvas. When you drag one out, a new Post-it of that color will immediately replace it in the dock.

   - **Edit Post-its:**  
     Click inside a Post-it to edit its content. The position pill (showing the relative position on the grid) updates automatically.

   - **Delete Post-its:**  
     A small "×" icon appears in the top left of each used Post-it (unless the Post-it is too close to the x- or y-axis). Click the icon to delete the Post-it.

   - **Upload Background:**  
     Click the "Upload Background" button in the toolbar to select an image file. The image will be applied as the whiteboard background, replacing the default grid.

   - **Save as PNG:**  
     When you are ready to save your work, click the "Save as PNG" button. The whiteboard (with all the Post-its and background) will be captured as a PNG image.

## Technologies Used

- **HTML5** for structure
- **CSS3** for styling (with Materialize CSS for basic styling)
- **Vanilla JavaScript** for interactivity
- **html2canvas** for capturing the whiteboard as a PNG

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! If you have ideas or improvements, please open an issue or submit a pull request.

## Acknowledgments

- [Materialize CSS](https://materializecss.com/) for the styling framework.
- [html2canvas](https://html2canvas.hertzen.com/) for enabling PNG export.
