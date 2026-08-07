A comprehensive analytics dashboard for visualizing and analyzing pothole detection data from CSV files. This application provides real-time statistics, graphical analysis, and support for multiple datasets to help infrastructure teams monitor and prioritize road maintenance efforts.

Features
CSV Data Upload: Upload pothole detection reports in CSV format

Real-time Statistics: View key metrics including total potholes, severity distribution, and location data

Interactive Visualizations: Dynamic charts and graphs for data analysis

Multi-dataset Support: Work with multiple data files simultaneously

Responsive Design: Optimized for both desktop and mobile viewing

Technology Stack
Frontend Framework: React 19 with TypeScript

Styling: Tailwind CSS 4.1

Charts & Visualizations: Recharts 3.8

CSV Processing: Papaparse 5.5

Build Tool: Vite 6.2

Animation: Motion (Framer Motion) 12.23

Icons: Lucide React 0.546

Installation
Prerequisites
Node.js (v18 or higher)

npm or yarn package manager

Setup
Clone the repository:

bash
git clone <repository-url>
cd pothole-detection-dashboard
Install dependencies:

bash
npm install
Create a .env.local file in the root directory:

bash
GEMINI_API_KEY=your_gemini_api_key_here
Start the development server:

bash
npm run dev
Open your browser and navigate to:

text
http://localhost:3000
Project Structure
text
├── src/
│   ├── components/     # Reusable UI components
│   ├── pages/          # Main application pages
│   ├── hooks/          # Custom React hooks
│   ├── utils/          # Helper functions
│   └── styles/         # Global styles and Tailwind config
├── public/             # Static assets
├── .env.example        # Environment variables template
├── index.html          # Entry HTML file
├── package.json        # Dependencies and scripts
├── tsconfig.json       # TypeScript configuration
├── vite.config.ts      # Vite build configuration
└── README.md           # Project documentation
Available Scripts
npm run dev - Start development server with hot reload

npm run build - Build for production

npm run preview - Preview production build locally

npm run clean - Remove build artifacts

npm run lint - Run TypeScript type checking

Environment Variables
Variable	Description
GEMINI_API_KEY	Required for AI-powered data analysis features
APP_URL	Application URL (auto-injected in production)
Deployment
The application is designed to be deployed on Google AI Studio or any platform that supports static React applications.

Build for Production
bash
npm run build
The build output will be in the dist/ directory.

Deploy to Google AI Studio
Push your code to a repository

Connect your repository to AI Studio

The platform will automatically build and deploy your application

Data Format
The dashboard expects CSV files with the following columns (at minimum):

Coordinates: Latitude and longitude of detected potholes

Severity: Classification of pothole severity (e.g., minor, moderate, severe)

Timestamp: Date and time of detection

Location: Street or area name

Contributing
Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

License
This project is proprietary and confidential. Unauthorized copying, distribution, or use is strictly prohibited.

Support
For support, questions, or bug reports, please contact the development team.
