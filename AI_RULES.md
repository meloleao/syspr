# AI Editor Rules and Guidelines

This document outlines the technical stack and specific development rules for maintaining and extending this application.

## Tech Stack Overview

*   **Framework:** React
*   **Language:** TypeScript
*   **Routing:** React Router (Routes are managed primarily in `src/App.tsx`).
*   **Styling:** Tailwind CSS (Utility-first approach, all designs must be responsive).
*   **UI Library:** shadcn/ui (Built on Radix UI primitives).
*   **Icons:** `lucide-react`.
*   **Project Structure:** Source code resides in `src/`. Pages are located in `src/pages/`, and reusable components are in `src/components/`.
*   **Component Philosophy:** Components must be small, focused, and generally kept under 100 lines of code. New components must always be created in new files.

## Library Usage Rules

1.  **UI Components:**
    *   **Mandatory:** Use components provided by `shadcn/ui` whenever possible.
    *   **Customization:** Do not edit the source files of `shadcn/ui` components. If customization is required, create a new component that wraps or extends the base component.
2.  **Styling:**
    *   **Mandatory:** All styling must be implemented using Tailwind CSS utility classes.
    *   **Responsiveness:** Designs must be responsive by default.
3.  **Icons:**
    *   **Mandatory:** Use icons exclusively from the `lucide-react` package.
4.  **Notifications:**
    *   Use a toast notification system to inform users about important events (success, error, loading).
5.  **File Structure:**
    *   Pages must be placed in `src/pages/`.
    *   Reusable components must be placed in `src/components/`.
    *   Directory names must be all lower-case.