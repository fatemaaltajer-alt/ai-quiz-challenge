# AI Specialist Badge Challenge

This is an interactive quiz designed to test your knowledge of AI concepts, safety, and ethics.

## How to Play Locally

To run this game on your local machine, you need to serve the files using a simple web server. You cannot open the `index.html` file directly in your browser due to security restrictions (CORS policy) that prevent modern JavaScript modules from loading this way.

### Prerequisites

- A modern web browser (like Chrome, Firefox, or Edge).
- Python 3 installed on your system (most macOS and Linux systems have it pre-installed).

### Setup & Running the Game

1.  **Download the Files**: Make sure you have all the project files (`index.html`, `index.tsx`, `App.tsx`, etc.) in a single folder.

2.  **Create an `assets` folder**: Inside your project folder, create a new folder named `assets`.

3.  **Add Images**: Place the required image files inside the `assets` folder:
    - `Water-Cycle-AI.png`
    - `AI-Scam-Email.jpg`
    - `PE-Project.png`
    - `Project-1.png`
    - `Project-2.JPG`
    - `Project-3.png`

4.  **Start a Local Server**:
    - Open a terminal or command prompt.
    - Navigate to the root directory of the project folder (the one containing `index.html`).
    - Run the following command:
      ```bash
      python3 -m http.server
      ```
    - If you have an older version of Python, you might need to use:
      ```bash
      python -m SimpleHTTPServer
      ```

5.  **Open the Game**:
    - The terminal will show a message like `Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/)`.
    - Open your web browser and go to the address: `http://localhost:8000`.

You should now see the "AI Specialist Badge Challenge" welcome screen and be able to play the game!

---

## Deploying to GitHub Pages

GitHub Pages is an excellent way to host this project for free. It will act as the web server for you.

1.  **Create a GitHub Repository**: Create a new public repository on GitHub and upload all the project files and folders (`index.html`, the `components` folder, the `assets` folder, etc.). The file structure should look like this in your repository:
    ```
    .
    ├── assets/
    │   ├── AI-Scam-Email.jpg
    │   ├── PE-Project.png
    │   ├── Project-1.png
    │   ├── Project-2.JPG
    │   ├── Project-3.png
    │   └── Water-Cycle-AI.png
    ├── components/
    │   ├── Badge.tsx
    │   └── QuizStages.tsx
    ├── App.tsx
    ├── constants.ts
    ├── index.html
    ├── index.tsx
    ├── metadata.json
    ├── README.md
    └── types.ts
    ```

2.  **Enable GitHub Pages**:
    - In your repository, go to `Settings` > `Pages`.
    - Under "Build and deployment", for the "Source", select `Deploy from a branch`.
    - For the "Branch", select `main` (or `master`) and keep the folder as `/ (root)`. Click `Save`.

3.  **Access Your Game**:
    - GitHub will provide you with a URL, usually in the format `https://<your-username>.github.io/<your-repository-name>/`.
    - It might take a few minutes for the site to become live.
    - Once it's ready, you can visit the URL and play the game directly in your browser.