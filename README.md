# 📲 alx-rick-and-morty-app

A Next.js application demonstrating **GraphQL integration** using Apollo Client to fetch and display **Rick and Morty episodes**. Built with **TypeScript**, **Tailwind CSS**, and **ESLint** for modern React development practices.

This repository contains queries, JSON outputs, and a React/Next.js application demonstrating GraphQL data fetching, pagination, and reusable components.

---

## 📁 Project Structure

- `graphql/`
  - `apolloClient.ts` → Apollo Client setup
  - `queries.ts` → GraphQL queries for episodes
- `pages/_app.tsx` → Wraps the app with ApolloProvider
- `pages/` → React components and pages (to be added in Part 4)
- `styles/` → Tailwind CSS styles


## 🛠 Installation & Setup

### 1. Clone the repository
```
git clone <https://github.com/BenTachie/alx-graphql-0x01>
cd alx-graphql-0x01/alx-rick-and-morty-app

2. Install dependencies
npm install @apollo/client graphql
npm install @types/graphql
npm install

3. Run the development server
npm run dev

Open http://localhost:3000 to view the app.
```

## 📜 How to Run GraphQL Queries
```
Example: Fetch a character by page
query {
  episodes(page: 1) {
    info {
      pages
      next
      prev
      count
    }
    results {
      id
      name
      air_date
      episode
    }
  }
}

Generate JSON output via endpoint:
https://rickandmortyapi.com/graphql
```
## 🚀 Features
- GraphQL queries for characters and episodes (by ID and paginated list)
- Reusable components for displaying episode cards
- Dynamic pagination and data fetching
- TypeScript interfaces for type safety

## 📚 Learning Objectives

- Understand GraphQL queries and schema
- Learn to query APIs with Apollo Client
- Apply GraphQL in React/Next.js environment
- Build modular, reusable, and scalable frontend components
- Manage paginated data and state effectively

## ⚡ Contributing

- Fork the repo
- Create a new branch (git checkout -b feature/my-feature)
- Make your changes
- Commit with a clear message
- Push and create a pull request

## 📄 License
MIT License

## Happy GraphQuesting! 🚀
