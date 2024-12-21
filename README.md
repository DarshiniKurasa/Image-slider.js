# Image Gallery with Horizontal Scrolling and Smooth Navigation

This project is a responsive image gallery featuring smooth horizontal scrolling, button navigation, and hover effects. It provides a user-friendly way to explore images with a modern design and intuitive controls.

## Features

- **Horizontal Scrolling**: Scroll through the gallery horizontally using the mouse wheel.
- **Smooth Navigation**: Navigate the gallery using "Next" and "Back" buttons with smooth scrolling behavior.
- **Hover Effects**: Images scale up and display full color on hover, providing an interactive experience.
- **Responsive Design**: The gallery layout adapts to different screen sizes for a seamless user experience.
- **Custom Scrollbar**: Scrollbar is hidden for a clean, minimalist look.

---

## Technologies Used

- **HTML5**: Semantic markup for structuring the gallery and navigation elements.
- **CSS3**: Modern styling with grid layout, transitions, and hover effects.
- **JavaScript**: Dynamic scrolling and button navigation functionality.

---

## Setup and Usage

### Prerequisites
Make sure you have the following:
- A web browser (e.g., Chrome, Firefox, Edge)
- A local or remote server to serve the HTML file (optional for local testing)

### Steps to Use
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/image-gallery.git
   cd image-gallery
   ```

2. **Add Images**
   Place your images inside the `images` folder. Ensure they are named appropriately (`image-1.png`, `image-2.png`, etc.).

3. **Open the Project**
   - Open `index.html` in your browser directly or using a local server.

---

## Folder Structure

```plaintext
├── images/                # Contains all gallery images and navigation icons
│   ├── image-1.png
│   ├── image-2.png
│   ├── ...
├── style.css              # Contains the CSS for styling the gallery
├── index.html             # Main HTML file
└── README.md              # Project documentation
```

---

## How It Works

1. **Horizontal Scrolling**: 
   - The gallery listens for `wheel` events, allowing horizontal scrolling when the mouse wheel is used. 
   - The scrolling behavior is dynamically adjusted for smoothness and speed.

2. **Button Navigation**:
   - "Next" and "Back" buttons allow users to scroll 900px forward or backward in the gallery with smooth animation.

3. **Hover Effects**:
   - Images use a grayscale filter by default. On hover, they display full color and scale up slightly, creating a lively effect.

4. **Custom Scrollbar**:
   - The `::-webkit-scrollbar` property hides the default scrollbar for a cleaner look.

---

## Customization

### Modify Scrolling Distance
To change the distance scrolled by buttons, adjust the values in the JavaScript code:
```javascript
scrollCont.scrollLeft += 900; // Scroll forward by 900px
scrollCont.scrollLeft -= 900; // Scroll backward by 900px
```

### Add/Remove Images
- Add new `<span>` elements with `<img>` tags inside the `.gallery div` in `index.html`.
- Ensure your images are placed in the `images` folder.

---

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute it.
