WEBVISION 2.0
Team Name - Logic Legends
Team Members - Shoham, Krish, Priyanshu

**ChatGPT Reimagined — A Tile-Based Glass OS for Thinking**

**Summary:**

Current chat interfaces like ChatGPT are built as a single, endless vertical list. After a hundred conversations, they become unmanageable and disconnected, even when multiple chats are about the same project. ChatGPT Reimagined solves this by turning every conversation into a spatial object — a Tile — on a dark, glassmorphic canvas. Instead of scrolling a list, you manage a visual board of your thoughts. Similar chats are automatically clubbed into Folders, or you can manually drag and drop tiles into a folder. When a folder is opened, it doesn't just show a list; it shows an AI-generated summary of all conversations inside it on the main view, with the original source chats available on the side for reference. It's designed as a frontend-only operating system for now, with a beautiful dark UI and frosted glass effects behind tiles, where the LLM API can be plugged in later via a local .env file. The goal is to move from a chatbot to a thought-management system.

**Core Features:**

**1. Design System - Dark + Glass:**
Dark base with semi-transparent tiles, backdrop blur, subtle borders and soft glow on hover to create depth and focus.

**2. Tile-Based Chat System:**
Every chat is an interactive tile showing title, preview, and tags, instead of a list item. The entire center canvas is a draggable board.

**3. Smart Foldering / Clubbing:**
- **Auto-Clustering:** System groups similar topics into folders.
- **Manual Drag & Drop:** Drag one tile onto another to create a folder, or drop a tile into an existing folder.

**4. Folder Summary View:**
On clicking a folder, split view opens:
- **Front Panel:** A synthesized summary of all chats inside the folder.
- **Side Panel:** List of source chats for provenance and quick access.

**5. Top Navigation Bar:**
Minimal horizontal OS-like bar: [New Chat] as primary CTA, then Apps, Agents, Settings, and Profile on the far right corner.

**6. Bottom Command Bar:**
A Spotlight-style search bar at the bottom, always focused. Primary input for new chats and search.
Advanced options inside: Connect Apps (@ Notion, @Gmail), Toggle Web Search, Open Website Directly, Call Agents (/researcher).

**7. Superstructure (Frontend Only):**
Built in Next.js with dummy data and workflows. Central state for tiles/folders. `.env.local` placeholder ready for LLM API integration. Real clustering, summarization, and persistence marked as Phase 2.
