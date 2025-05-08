# Traffic Security Surveillance System for India

A Next.js application for monitoring and reporting traffic incidents across India, finding alternative routes, and analyzing traffic patterns.

## Features

- Real-time traffic incident monitoring on an interactive map
- Incident reporting with geolocation support
- Alternative route finding to avoid traffic incidents
- Traffic analytics and incident hotspot identification
- User authentication system

## Prerequisites

- Node.js 18.x or later
- npm or yarn
- PostgreSQL (optional - the app works without a database using sample data)

## Installation

### 1. Clone the repository

\`\`\`bash
git clone https://github.com/yourusername/traffic-surveillance.git
cd traffic-surveillance
\`\`\`

### 2. Install dependencies

\`\`\`bash
npm install
# or
yarn install
\`\`\`

### 3. Set up environment variables

Create a `.env.local` file in the root directory with the following variables:

\`\`\`
# PostgreSQL connection (optional)
POSTGRES_URL=your_postgres_connection_string
POSTGRES_URL_NON_POOLING=your_postgres_non_pooling_connection_string

# For production, add these as well
NEXTAUTH_URL=your_app_url
NEXTAUTH_SECRET=your_secret_key
\`\`\`

Note: The application will work without PostgreSQL by using sample data.

### 4. Set up the database (optional)

If you want to use PostgreSQL:

1. Create a PostgreSQL database
2. Run the schema.sql file to create the necessary tables:

\`\`\`bash
psql -U your_username -d your_database_name -a -f schema.sql
\`\`\`

## Running the Application

### Development mode

\`\`\`bash
npm run dev
# or
yarn dev
\`\`\`

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Production build

\`\`\`bash
npm run build
npm start
# or
yarn build
yarn start
\`\`\`

## Deployment

This project can be easily deployed to Vercel:

1. Push your code to a GitHub repository
2. Import the project in Vercel
3. Set up the environment variables in the Vercel dashboard
4. Deploy

## Project Structure

- `/app` - Next.js App Router pages and layouts
- `/components` - React components
- `/lib` - Utility functions and server actions
- `/public` - Static assets

## Technologies Used

- Next.js 14 with App Router
- React 18
- TypeScript
- Tailwind CSS
- shadcn/ui components
- Leaflet for maps
- PostgreSQL (optional)
- Vercel for deployment

## License

MIT
