# nextjs-client-components

This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Description

`nextjs-client-components` is a modern web application built with [Next.js](https://nextjs.org). It demonstrates the use of **Client Components**, such as a reusable `Button` component, to handle interactivity in a modern web application. This project also highlights the difference between server and client components.

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- npm, yarn, or pnpm (depending on your preference)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Achintha-999/nextjs-client-components.git

2. Navigate to the project directory:    
   cd nextjs-client-components

3. Install dependencies:
   npm install
# or
yarn install
# or
pnpm install

Running the Development Server
Start the development server:

npm run dev
# or
yarn dev
# or
pnpm dev

Open http://localhost:3000 in your browser to view the app.

Client Components
This project includes client components, which are interactive and rendered on the client side. For example, the Button component is a client component imported and used in the Home component.

Example of Client Component Usage
In page.jsx:
import Button from "./(components)/Button";

export default function Home() {
  return (
    <>
      <h3>Server Components vs Client Components</h3>
      <Button />
    </>
  );
}

he Button component is located in the src/app/(components)/Button.jsx directory and is designed to handle client-side interactions.

Example of the Button Component
The Button component is explicitly marked as a client component using the "use client" directive:

// filepath: /src/app/(components)/Button.jsx
"use client";

export default function Button() {
  const handleClick = () => {
    alert("Button clicked!");
  };

  return <button onClick={handleClick}>Click Me</button>;
}

Key Features of Client Components:
Interactivity: Client Components allow you to add event listeners and handle user interactions.
Rendering: Unlike Server Components, Client Components are rendered in the browser.
Usage: To use a Client Component, ensure it is marked with the "use client" directive at the top of the file.
Project Structure
The project structure is as follows:

nextjs-client-components/
├── .gitignore
├── .next/
├── eslint.config.mjs
├── jsconfig.json
├── next.config.mjs
├── package.json
├── public/
├── README.md
├── src/
│   └── app/
│       ├── (components)/
│       │   └── Button.jsx
│       └── page.jsx

Learn More
To learn more about Next.js and Client Components, check out the following resources:

Next.js Documentation - Learn about Next.js features and API.
Client and Server Components - Learn about the difference between Client and Server Components.
License
This project is open-source and available under the MIT License. ```
