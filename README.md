# Band Name Generator 🎸

The **Band Name Generator** is a fun, interactive web application that generates random band names by combining an adjective and a noun. It uses **Node.js**, **Express**, and **EJS** for dynamic content rendering.

## Features

- Generate random, creative band names with the click of a button.
- Dynamic rendering of generated names using EJS.
- Responsive design with static CSS files for styling.
- Dynamic year in the footer to keep the page up-to-date.

## Technologies Used

- **Node.js**: Backend JavaScript runtime.
- **Express**: Lightweight and flexible web application framework.
- **EJS**: Embedded JavaScript for dynamic templating.
- **CSS**: Styling for the application.
- **Body-Parser**: Middleware to parse form submissions.

## Prerequisites

1. **Node.js**: Download and install from [Node.js official site](https://nodejs.org/).
2. **npm**: Comes with Node.js installation for managing dependencies.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/band-name-generator.git
   cd band-name-generator
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create the necessary file structure:
   - Place your CSS files in the `public` folder.
   - Use the provided `partials` folder for header and footer EJS templates.

4. Start the server:
   ```bash
   node index.js
   ```

5. Open your browser and navigate to:
   ```bash
   http://localhost:3000
   ```

## File structure

```bash
project/
│
├── index.js            # Main application logic
├── views/
│   ├── index.ejs       # Main EJS template
│   ├── partials/
│       ├── header.ejs  # Header partial template
│       ├── footer.ejs  # Footer partial template
├── public/
│   └── styles/
│       └── main.css    # Static CSS file
├── package.json        # Project metadata and dependencies
```

## How It Works

1. The home page (`index.ejs`) displays a default welcome message.
2. When the "Generate Name" button is clicked, the form submission triggers a `POST` request to `/submit`.
3. The server randomly selects an adjective and a noun from predefined arrays and renders the `index.ejs` template with these values.
4. The generated band name is displayed dynamically on the page.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

