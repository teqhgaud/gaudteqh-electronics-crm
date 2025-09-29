# Gaudteqh Electronics CRM - Setup Instructions

## Prerequisites

Before running the CRM application, you need to install the following:

### 1. Install Node.js

1. Go to [https://nodejs.org](https://nodejs.org)
2. Download the **LTS version** (Long Term Support)
3. Run the installer and follow the setup wizard
4. **Important**: Make sure to check "Add to PATH" during installation
5. Restart your terminal/PowerShell after installation

### 2. Verify Installation

Open a new terminal/PowerShell window and run:
```bash
node --version
npm --version
```

Both commands should return version numbers.

## Quick Start

Once Node.js is installed, run these commands in your project directory:

```bash
# Install all dependencies
npm run install-all

# Copy environment file
copy .env.example .env

# Start the development servers
npm run dev
```

## Manual Setup (Alternative)

If you prefer to set up each part manually:

```bash
# Install root dependencies
npm install

# Install client dependencies
cd client
npm install
cd ..

# Install server dependencies
cd server
npm install
cd ..

# Start both client and server
npm run dev
```

## Access the Application

- **Frontend (React)**: http://localhost:3000
- **Backend API**: http://localhost:5000

## Troubleshooting

### Node.js not found
- Make sure Node.js is installed and added to PATH
- Restart your terminal after installation
- Try running `refreshenv` in PowerShell if using Chocolatey

### Port already in use
- Make sure ports 3000 and 5000 are available
- Check if other applications are using these ports

### Dependencies issues
- Delete `node_modules` folders and `package-lock.json` files
- Run `npm install` again

## Next Steps

After the application is running:
1. Open http://localhost:3000 in your browser
2. The CRM interface should load
3. Start developing your features!

## Support

If you encounter any issues, check the GitHub repository:
https://github.com/teqhgaud/gaudteqh-electronics-crm
