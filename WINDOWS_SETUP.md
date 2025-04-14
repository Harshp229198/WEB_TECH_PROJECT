# Running Rhythmix on Windows

This guide provides detailed instructions for running the Rhythmix music application on Windows systems.

## Common Windows Issues

Windows handles environment variables and command execution differently than Unix-based systems. This can lead to errors like:

- `'NODE_ENV' is not recognized as an internal or external command`
- `Error: listen ENOTSUP: operation not supported on socket 0.0.0.0:5000`

## Method 1: Using VS Code (Recommended)

1. Open the project in VS Code
2. Press `F5` or click the "Run and Debug" icon in the side panel
3. Select "Launch Rhythmix (Windows)" from the dropdown menu
4. Click the green play button
5. The app will start on port 3000

## Method 2: Using the Batch File

We've included a batch file specifically for Windows users:

1. Open Windows Explorer and navigate to your project folder
2. Double-click on `start-dev.bat`
3. A command prompt window will open and run the application
4. The app will be available at http://localhost:3000

## Method 3: Using Command Prompt Manually

1. Open Command Prompt (cmd)
2. Navigate to your project directory:
   ```
   cd C:\path\to\your\project
   ```
3. Set the environment variables and run the application:
   ```
   set NODE_ENV=development
   set PORT=3000
   npx tsx server/index.ts
   ```

## Method 4: Using PowerShell

1. Open PowerShell
2. Navigate to your project directory:
   ```
   cd C:\path\to\your\project
   ```
3. Set the environment variables and run the application:
   ```
   $env:NODE_ENV = "development"
   $env:PORT = "3000"
   npx tsx server/index.ts
   ```

## Troubleshooting

### Port Issues

If you still encounter port binding issues:

- Try a different port by changing the PORT value in the commands above
- Check if you have other applications using port 3000
- Try closing any other Node.js applications

### Module Not Found

If you get errors about missing modules:

1. Make sure all dependencies are installed:
   ```
   npm install
   ```

### Node.js Version

Make sure you have Node.js v14 or higher installed:

1. Check your version:
   ```
   node --version
   ```
2. If necessary, download the latest version from [nodejs.org](https://nodejs.org)

## Additional Notes

- The application uses JWT for authentication
- All API routes are prefixed with `/api`
- Static assets are served from the `public` directory
