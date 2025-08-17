Rust + WebAssembly News Fetcher

A high-performance, browser-based news client that fetches and displays the latest headlines on technology and cryptocurrency. This application uses a Rust core, compiled to WebAssembly, to interact with the Benzinga API, demonstrating a modern approach to building fast and efficient web applications.

Features
Dynamic Topic Search: Enter any topic channel supported by the Benzinga API (e.g., CRYPTO, TECH, MARKETS) to get the latest news.
Real-Time Data: Fetches the 20 most recent articles directly from the Benzinga API.
Clean & Responsive UI: A modern, easy-to-read interface built with Tailwind CSS that works on both desktop and mobile.
High-Performance Core: The entire logic for making and parsing the API request is handled by a Rust module running at near-native speed via WebAssembly.

Tech Stack
This project showcases a powerful combination of systems programming and modern web technologies.

Core Logic: Rust

Browser Target: WebAssembly (Wasm)

API Interaction: reqwest for asynchronous HTTP requests.

Data Handling: serde and serde_json for robust JSON parsing.

Rust-to-Wasm Bridge: wasm-pack and wasm-bindgen.

Frontend: HTML5, JavaScript

Styling: Tailwind CSS

Getting Started
To run this project on your local machine, you will need to have the Rust toolchain, wasm-pack, and a valid Benzinga API key.

Prerequisites
Install Rust:
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh


Install wasm-pack:
cargo install wasm-pack


Get a Benzinga API Key: Sign up for a developer account at Benzinga Cloud to get your free trial API key.
Installation & Running
Clone the repository:
git clone https://github.com/your-username/news-webapp.git
cd news-webapp


Add Your API Key: Open the index.html file and replace the placeholder "YOUR_API_KEY_HERE" on line 56 with your actual Benzinga API key.
Build the WebAssembly package: This command compiles the Rust code and generates the necessary JavaScript bindings in a pkg directory.
wasm-pack build --target web


Start a local web server: The project must be served over http://. 

A simple Python server is perfect for this.
python3 -m http.server


Open the application: Open your web browser and navigate to http://localhost:8000.

Acknowledgements
This project was developed by Jeremy Royer in collaboration with Google's Gemini. The core logic, architecture, and debugging were a joint effort, showcasing a modern approach to AI-assisted development.

Project Lead & Developer: Jeremy Royer

AI Assistant & Pairing Partner: Google's Gemini
