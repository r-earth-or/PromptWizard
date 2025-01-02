# Web GUI for Prompt Optimization

This project provides a simple web GUI for prompt optimization using Vue.js and Vite for the frontend, and FastAPI for the backend. The project also includes a Dockerfile for easy deployment and environment variables for LLM configuration.

## Prerequisites

- Node.js and npm installed
- Docker installed

## Setup

1. Clone the repository:

```sh
git clone https://github.com/r-earth-or/PromptWizard.git
cd PromptWizard/demos/web-gui
```

2. Install frontend dependencies:

```sh
cd frontend
npm install
```

3. Create a `.env` file in the `demos/web-gui` directory and add the following environment variables:

```sh
OPENAI_API_VERSION=""
AZURE_OPENAI_ENDPOINT=""
AZURE_OPENAI_DEPLOYMENT_NAME=""
MODEL_TYPE="OPENAI"
OPENAI_API_KEY=""
BASE_URL=""
OPENAI_MODEL_NAME="gpt-4o"
```

4. Build and run the Docker container:

```sh
docker build -t promptwizard-web-gui .
docker run -p 80:80 promptwizard-web-gui
```

## Usage

1. Open your browser and navigate to `http://localhost`.

2. You should see the web GUI with input fields for the prompt and buttons to optimize the prompt.

3. Enter your prompt and click the "Optimize" button to get the optimized prompt and expert profile.

## Project Structure

- `frontend/`: Contains the Vue.js frontend code
  - `App.vue`: Main Vue.js component
  - `components/`: Directory for Vue.js components
    - `Header.vue`: Header component
    - `Footer.vue`: Footer component
    - `PromptInput.vue`: Prompt input component
    - `PromptOutput.vue`: Prompt output component
  - `main.js`: Entry point for the Vue.js application
  - `style.css`: CSS styles for the application
  - `index.html`: HTML template for the application
- `api/`: Contains the FastAPI backend code
  - `main.py`: FastAPI application file
- `Dockerfile`: Dockerfile for building the Docker image
- `.env`: Environment variables for LLM configuration

## Contributing

Feel free to submit issues, fork the repository and send pull requests!

## License

This project is licensed under the MIT License.
