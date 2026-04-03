# TrackWise - Personal Finance Tracker

TrackWise is a modern, intuitive, and feature-rich personal finance tracker designed to help you manage your money with ease. Gain clarity on your spending, track your income, and achieve your financial goals with a beautifully designed interface and powerful features.

some sample images are under the sample_image_folder;

## Features

- **Secure User Authentication**: Sign up, log in, and manage your account securely. Includes a password change feature.
- **Interactive Dashboard**: Get a quick overview of your financial health with a summary of total income, expenses, and current balance.
- **Comprehensive Transaction Management**:
  - Add, edit, and delete transactions with ease.
  - Assign categories, add optional descriptions, and set dates.
  - View a detailed list of all your transactions.
- **Advanced Filtering & Search**:
  - Filter transactions by type (income/expense), category, and custom date ranges.
  - Search functionality to quickly find specific transactions.
- **Customizable Categories**:
  - Create and manage your own income and expense categories.
  - Personalize categories with a vast, searchable icon library and a full-featured color picker.
- **In-depth Financial Reports**:
  - **Monthly Overview**: Detailed breakdown of income and expenses by category for any given month, complete with pie charts and data tables.
  - **Yearly Overview**: See the bigger picture with a year-over-year comparison of your financial activity, visualized with stacked bar charts.
- **Personalization & Accessibility**:
  - **Multi-Currency Support**: Choose from a list of currencies (USD, EUR, INR, JPY, GBP, AED), and have all values displayed in your preferred currency.
  - **Compact Number Formatting**: Toggle between standard number display (e.g., 1,000,000) and compact formatting (e.g., 1M or 10L) for improved readability.
  - **Light & Dark Mode**: Switch between themes to suit your preference.
  - **Responsive Design**: Fully responsive UI that works seamlessly on desktop, tablet, and mobile devices.
- **Data Export**: Download a CSV file of your filtered transactions at any time.

## Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) (with App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **UI**: [React](https://react.dev/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Component Library**: [ShadCN/UI](https://ui.shadcn.com/)
- **Database**: [MongoDB](https://www.mongodb.com/)
- **Authentication**: JWT-based session management

## Getting Started

Follow these instructions to get a local copy up and running.

### Prerequisites

- Node.js (v18 or newer recommended)
- npm or yarn
- A MongoDB database instance (local or cloud-hosted with [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/trackwise.git
    cd trackwise
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Set up environment variables:**
    Create a `.env.local` file in the root of your project and add the following variables:
    ```.env
    MONGODB_URI="your_mongodb_connection_string"
    JWT_SECRET="your_super_secret_jwt_key"
    ```
    - `MONGODB_URI`: Your connection string for your MongoDB database.
    - `JWT_SECRET`: A long, random, and secret string used for signing authentication tokens.

### Running the Application

1.  **Run the development server:**
    ```bash
    npm run dev
    ```
    The application will be available at `http://localhost:9002`.

2.  **Run the Genkit development server (for AI features):**
    Open a separate terminal and run:
    ```bash
    npm run genkit:watch
    ```

### Production Build

1.  **Build the application for production:**
    ```bash
    npm run build
    ```

2.  **Start the production server:**
    ```bash
    npm run start
    ```
    The application will be running in production mode.
