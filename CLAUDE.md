# AI Collaboration Guide

This document provides essential context for AI models interacting with this project. Adhering to these guidelines will ensure consistency and maintain code quality.

## 1. Project Overview & Purpose

* **Primary Goal:** This is a Next.js web application that serves as the frontend for a Twitter-like platform called "TwitterX". It's a React-based web application with server-side rendering capabilities.
* **Business Domain:** Social Media / Microblogging Platform

## 2. Core Technologies & Stack

* **Languages:** TypeScript, JavaScript
* **Frameworks & Runtimes:** 
  * Next.js 15.4.6 (App Router)
  * React 19.1.0
  * React DOM 19.1.0
* **Databases:** Not directly included in frontend (likely connects to backend APIs)
* **Key Libraries/Dependencies:** 
  * next/font (for font optimization)
  * Tailwind CSS v4 (for styling)
* **Package Manager(s):** pnpm

## 3. Architectural Patterns

* **Overall Architecture:** Next.js App Router architecture with server-side rendering capabilities. Component-based UI architecture with React.
* **Directory Structure Philosophy:**
    * `/src/app`: Contains all pages, layouts, and routing using Next.js App Router structure
    * `/public`: Static assets like images and icons
    * `/node_modules`: Dependencies managed by pnpm

## 4. Coding Conventions & Style Guide

* **Formatting:** 
  * Uses ESLint with Next.js core web vitals and TypeScript configurations
  * Indentation: 2 spaces (inferred from tsconfig.json and eslint config)
  * Follows Next.js and React best practices
* **Naming Conventions:**
    * Variables, functions: camelCase (inferred from source code)
    * Components: PascalCase (inferred from source code)
    * Files: kebab-case for page components, camelCase for others (inferred from source code)
* **API Design:** Client-side application that likely connects to backend APIs (not defined in this frontend project)
* **Error Handling:** Standard React/Next.js error handling patterns (not explicitly defined in current codebase)

## 5. Key Files & Entrypoints

* **Main Entrypoint(s):** `src/app/page.tsx` (home page), `src/app/layout.tsx` (root layout)
* **Configuration:** 
  * `next.config.ts` (Next.js configuration)
  * `tsconfig.json` (TypeScript configuration)
  * `eslint.config.mjs` (ESLint configuration)
  * `postcss.config.mjs` (PostCSS configuration)
  * `package.json` (Project dependencies and scripts)
* **CI/CD Pipeline:** Not configured in this project

## 6. Development & Testing Workflow

* **Local Development Environment:** 
  1. Install dependencies with `pnpm install`
  2. Run development server with `pnpm dev`
  3. Access application at http://localhost:3000
* **Testing:** No testing framework configured in this project
* **CI/CD Process:** No CI/CD pipeline configured in this project

## 7. Specific Instructions for AI Collaboration

* **Contribution Guidelines:** No explicit contribution guidelines found
* **Infrastructure (IaC):** No Infrastructure as Code directory found
* **Security:** 
  * Do not hardcode secrets or keys
  * Ensure any API calls follow security best practices
  * Follow React and Next.js security recommendations
* **Dependencies:** 
  * When adding new dependencies, use `pnpm add` for production dependencies or `pnpm add -D` for development dependencies
  * Update the `package.json` file accordingly
* **Commit Messages:** No specific commit message format defined in this project