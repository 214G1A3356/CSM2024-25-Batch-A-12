# Welcome to AUTOMATED SOFTWARE ENGINEER : HARNESSING AI TO REVOLUTIONIZE CODE GENERATION & SOFTWARE DEVELOPMENT

It allows you to choose the LLM that you use for each prompt! Currently, you can use OpenAI, Anthropic, Ollama, OpenRouter, Gemini, LMStudio, Mistral, xAI, HuggingFace, DeepSeek, or Groq models - and it is easily extended to use any other model supported by the Vercel AI SDK! See the instructions below for running this locally and extending it to include more models.


## Features

-   **AI-powered full-stack web development**  directly in your browser.
-   **Support for multiple LLMs**  with an extensible architecture to integrate additional models.
-   **Attach images to prompts**  for better contextual understanding.
-   **Integrated terminal**  to view output of LLM-run commands.
-   **Revert code to earlier versions**  for easier debugging and quicker changes.
-   **Download projects as ZIP**  for easy portability.
-   **Integration-ready Docker support**  for a hassle-free setup.


## Setup

If you're new to installing software from GitHub, don't worry! If you encounter any issues, feel free to submit an "issue" using the provided links or improve this documentation by forking the repository, editing the instructions, and submitting a pull request. The following instruction will help you get the stable branch up and running on your local machine in no time.

### Prerequisites

1.  **Install Git**:  [Download Git](https://git-scm.com/downloads)
2.  **Install Node.js**:  [Download Node.js](https://nodejs.org/en/download/)
    
3.  After installation, the Node.js path is usually added to your system automatically. To verify:
    
    -   **Windows**: Search for "Edit the system environment variables," click "Environment Variables," and check if  `Node.js`  is in the  `Path`  variable.
    -   **Mac/Linux**: Open a terminal and run:
        
        `echo  $PATH` 
        
        Look for  `/usr/local/bin`  in the output.
### Clone the Repository
Clone the repository using Git:
  
      git  clone  https://github.com/214G1A3356/CSM2024-25-Batch-A-12.git
### Rename the folder name into " aswe "
      CSM2024-25-Batch-A-12 to aswe
the internally functionality was build on the folder name with aswe 
### Entering API Keys

#### Configure API Keys Directly in the Application
Alternatively, you can configure your API keys directly in the application once it's running. To do this:

1.  Launch the application and navigate to the provider selection dropdown.
2.  Select the provider you wish to configure.
3.  Click the pencil icon next to the selected provider.
4.  Enter your API key in the provided field.

This method allows you to easily add or update your keys without needing to modify files directly.

Once you've configured your keys, the application will be ready to use the selected LLMs.
## Run the Application
1.  **Install Dependencies**:
				
		pnpm install 

		
	If  `pnpm`  is not installed, install it using:
	
		sudo  npm  install  -g  pnpm 

1.  **Start the Application**:
    
	    pnpm  run  dev
    
    This will start the Remix Vite development server. You will need Google Chrome Canary to run this locally if you use Chrome! It's an easy install and a good browser for web development anyway.
    

## Available Scripts
-   `pnpm run dev`: Starts the development server.
-   `pnpm run build`: Builds the project.
-   `pnpm run start`: Runs the built application locally using Wrangler Pages. This script uses  `bindings.sh`  to set up necessary bindings so you don't have to duplicate environment variables.
-   `pnpm run preview`: Builds the project and then starts it locally, useful for testing the production build. Note, HTTP streaming currently doesn't work as expected with  `wrangler pages dev`.
-   `pnpm test`: Runs the test suite using Vitest.
-   `pnpm run typecheck`: Runs TypeScript type checking.
-   `pnpm run typegen`: Generates TypeScript types using Wrangler.
-   `pnpm run deploy`: Builds the project and deploys it to Cloudflare Pages.

## Development

To start the development server:

	pnpm  run  dev

This will start the Remix Vite development server. You will need Google Chrome Canary to run this locally if you use Chrome! It's an easy install and a good browser for web development anyway.

## Tips and Tricks

Here are some tips to get the most out of bolt.diy:

-   **Be specific about your stack**: If you want to use specific frameworks or libraries (like Astro, Tailwind, ShadCN, or any other popular JavaScript framework), mention them in your initial prompt to ensure Bolt scaffolds the project accordingly.
    
-   **Use the enhance prompt icon**: Before sending your prompt, try clicking the 'enhance' icon to have the AI model help you refine your prompt, then edit the results before submitting.
    
-   **Scaffold the basics first, then add features**: Make sure the basic structure of your application is in place before diving into more advanced functionality. This helps Bolt understand the foundation of your project and ensure everything is wired up right before building out more advanced functionality.
    
-   **Batch simple instructions**: Save time by combining simple instructions into one message. For example, you can ask Bolt to change the color scheme, add mobile responsiveness, and restart the dev server, all in one go saving you time and reducing API credit consumption significantly.
    

