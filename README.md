# shopify
This project is a product page for "Shopify" designed to showcase a product with an interactive gallery, variant selection (color and size), product details, and related product sections.

**Features Implemented
Product Gallery:**
Displays a main image with a thumbnail gallery.
Thumbnails are clickable to update the main image.
Two thumbnails per color (Black, White, Blue) are dynamically loaded when a color is selected.
**Variant Selection:**
Color selection with swatches (Black, White, Blue) that update the gallery and description.
Size selection dropdown with options (S, M, L, XL).
Selections are saved to localStorage for persistence across page reloads.
**Product Details:**
Tabs for Description, Product Information, and Shipping Details.
Description updates dynamically based on the selected color.
**Modals:**
Size Chart modal with a table of measurements.
Compare Colors modal showing color swatches.
Modals can be closed via a close button, overlay click, or ESC key.
**Additional Sections:**
Product Bundle section with a curated set of items and a total price.
Pair Well With carousel for complementary products.
Related Products grid with badges for "New" and "Popular" items.
**Responsive Design:**
Layout adjusts for different screen sizes (desktop, tablet, mobile).
Thumbnails and product sections stack on smaller screens.
How to Run Locally
Clone or Download the Project:
Clone the repository or download the project files to your local machine.
**Set Up a Local Server:**
Since the project uses relative paths (e.g., css/styles.css, js/scripts.js, assets/), you need to serve the files through a local server to avoid CORS issues.
Use a simple HTTP server like:
Python: If you have Python installed, navigate to the project directory and run:
python -m http.server 8000
Node.js: If you have Node.js installed, you can use http-server:
npm install -g http-server
http-server
Alternatively, use a browser extension or IDE feature (e.g., VS Code’s Live Server).
**Access the Page:**
Open your browser and navigate to http://localhost:8000 (or the port provided by your server).
The index.html file will load the product page.
Interact with the Page:
Click on thumbnails to update the main image.
Select a color to update the thumbnails and description.
Use the Size Chart and Compare Colors buttons to view modals.
Explore the Product Bundle, Pair Well With, and Related Products sections.

**Folder Structure
**Product-page/**
├── index.html        # Main HTML file for the product page
├── README.md         # Project documentation
├── css/
│   └── styles.css    # CSS styles for the product page
├── js/
│   └── scripts.js    # JavaScript for dynamic functionality
├── assets/           # Folder for images (placeholders used in this project)
│   ├── black.jpg     # Placeholder: https://via.placeholder.com/60/000
│   ├── black2.jpg    # Placeholder: https://via.placeholder.com/60/111
│   ├── white1.jpg    # Placeholder: https://via.placeholder.com/60/fff
│   ├── white2.jpg    # Placeholder: https://via.placeholder.com/60/eee
│   ├── blue1.jpg     # Placeholder: https://via.placeholder.com/60/1e90ff
│   ├── blue2.jpg     # Placeholder: https://via.placeholder.com/60/4682b4
│   ├── classictee.jpg # Placeholder: https://via.placeholder.com/150
│   ├── jeans.jpg     # Placeholder: https://via.placeholder.com/150/333
│   ├── belt.jpg      # Placeholder: https://via.placeholder.com/150/666
│   ├── denimjacket.jpg # Placeholder: https://via.placeholder.com/200
│   ├── chino.jpg     # Placeholder: https://via.placeholder.com/200/333
│   ├── sneakers.jpg  # Placeholder: https://via.placeholder.com/200/666
│   ├── sunglasses.jpg # Placeholder: https://via.placeholder.com/200/999
│   ├── polo.jpg      # Placeholder: https://via.placeholder.com/200
│   ├── hoodie.jpg    # Placeholder: https://via.placeholder.com/200/333
│   ├── shorts.jpg    # Placeholder: https://via.placeholder.com/200/666
│   └── cap.jpg       # Placeholder: https://via.placeholder.com/200/999

**Notes**
Images: The project uses via.placeholder.com placeholders for all images. In a real application, replace these paths in index.html and scripts.js with actual image files in the assets/ folder.
Local Server Requirement: Running the project directly by opening index.html in a browser (via file://) may cause issues with loading resources due to CORS policies. A local server is recommended.
