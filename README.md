
# Project Initialization Kit

Welcome to the **Project Initialization Kit**, a comprehensive setup template designed to streamline your project setup process. This template supports modern development stacks and tools, including Node.js, React, TypeScript, MongoDB, Docker, and Docker Compose. By following these steps, you can quickly bootstrap your project and focus on development.

## Features

- **Node.js & React.js**: Ready for server and client-side development.
- **TypeScript**: Type safety for better code quality and maintainability.
- **MongoDB**: Pre-configured for your database needs.
- **Docker & Docker Compose**: Containerization and orchestration setup.
- **ESLint**: Ensures code quality and consistency.
- **Prettier**: Code formatting for a clean codebase.
- **Husky**: Git hooks for enforcing code quality before commits and pushes.
- **Commitlint**: Enforces conventional commit messages for a clean and consistent commit history.

## Getting Started

Follow these steps to set up your project:

1. **Clone the Repository**

   ```bash
   git clone https://github.com/manishdashsharma/project-setup-starter.git <your-folder-name>
   ```

   Example:

   ```bash
   git clone https://github.com/manishdashsharma/project-setup-starter.git myapp
   ```

2. **Create a Remote Repository**

   After cloning the repository locally, create a new repository on your Git hosting platform (e.g., GitHub, GitLab).

3. **Set Execution Permission for Setup Script**

   Navigate to the project folder and give the setup script execution permission:

   ```bash
   cd <your-folder-name>
   chmod +x setup_application.sh
   ```

4. **Run the Setup Script**

   Run the setup script to automate the initialization process:

   ```bash
   ./setup_application.sh
   ```

   This script will:

   - Remove the existing `.git` folder
   - Install dependencies
   - Initialize Git and Husky
   - Install both server and client dependencies
   - Set up necessary permissions for scripts

5. **Add Your Remote Repository**

   Once your new repository has been created, you can now add your remote repository URL:

   ```bash
   git branch -M main
   git remote add origin <your-remote-url>
   ```

   Make sure to replace `<your-remote-url>` with the actual URL of your newly created repository.

6. **Create Environment Files**

   After setting up the repository, manually create the environment files:

   - `.env.development`
   - `.env.production`

   Copy the content from `.env.example` into both files.

7. **Start Docker Client**

   Ensure Docker is running on your machine.

8. **Start the Server**

   Start the project by running the following script:

   ```bash
   ./start_application.sh
   ```

9. **Clean Up Docker Environment**

   To remove all Docker containers, images, volumes, and builds associated with the project, use the cleanup script:

   ```bash
   ./remove.sh
   ```

   **Note:** This script will remove all Docker services and data associated with the project. Ensure no other critical services are running in Docker before executing it.

## Check Your Setup

After completing the setup, verify if everything is running correctly by accessing the following:

- **Backend**: [http://localhost:5000/api/v1/self](http://localhost:5000/api/v1/self)
- **Frontend**: [http://localhost:5173](http://localhost:5173)

## Contributing

We welcome contributions to improve this template. Please fork the repository and submit a pull request with your enhancements.
