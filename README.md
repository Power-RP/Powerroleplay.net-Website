# 📖 Power Website — Complete Staff Guide

> **Website:** [https://powerroleplay.net](https://powerroleplay.net)  
> **FiveM Server:** [cfx.re/join/opvd97](https://cfx.re/join/opvd97)  
> **Discord:** [discord.gg/powerrp](https://discord.gg/powerrp)  
> **Last Updated:** February 2026

---

## Table of Contents

1. [Overview](#1-overview)
2. [Getting Started — Authentication & Login](#2-getting-started--authentication--login)
3. [The Homepage](#3-the-homepage)
4. [Navigation Bar](#4-navigation-bar)
5. [User Dashboard](#5-user-dashboard)
6. [Notifications System](#6-notifications-system)
7. [Power AI — AI Chat Assistant](#7-power-ai--ai-chat-assistant)
8. [Help Center](#8-help-center)
9. [Rulebook](#9-rulebook)
10. [Applications System](#10-applications-system)
    - [Application Types](#application-types)
    - [Submitting an Application](#submitting-an-application)
    - [Application Lifecycle](#application-lifecycle)
    - [AI Detection System](#ai-detection-system)
    - [Reviewing Applications (Staff)](#reviewing-applications-staff)
    - [Customizing Application Questions](#customizing-application-questions)
11. [Tickets (Support) System](#11-tickets-support-system)
    - [Creating a Ticket](#creating-a-ticket)
    - [Ticket Categories](#ticket-categories)
    - [Tebex Purchase Verification](#tebex-purchase-verification)
    - [Citizen ID Verification](#citizen-id-verification)
    - [Ticket Lifecycle & Statuses](#ticket-lifecycle--statuses)
    - [Discord DM Integration](#discord-dm-integration)
    - [Auto-Close System](#auto-close-system)
    - [Managing Tickets (Staff)](#managing-tickets-staff)
    - [AI Ticket Assistant](#ai-ticket-assistant)
12. [Divisions System](#12-divisions-system)
    - [Law Enforcement](#law-enforcement)
    - [Medical Services (EMS)](#medical-services-ems)
    - [Businesses](#businesses)
    - [Real Estate](#real-estate)
    - [Factions](#factions)
    - [Roster Management](#roster-management)
    - [Clock-In / Activity Tracking](#clock-in--activity-tracking)
    - [Division Permissions](#division-permissions)
13. [Staff Panel](#13-staff-panel)
    - [Staff Dashboard Tab](#staff-dashboard-tab)
    - [Support Tickets Tab](#support-tickets-tab)
    - [Manage Applications Tab](#manage-applications-tab)
    - [Manage Permissions Tab](#manage-permissions-tab)
    - [Application Editor Tab](#application-editor-tab)
    - [Staff Activity / Leaderboard Tab](#staff-activity--leaderboard-tab)
    - [Staff Handbook Tab](#staff-handbook-tab)
    - [Power AI Knowledge Base Tab](#power-ai-knowledge-base-tab)
    - [Send Announcement Tab](#send-announcement-tab)
14. [Permissions System — Complete Reference](#14-permissions-system--complete-reference)
    - [How Permissions Work](#how-permissions-work)
    - [Full Permission List](#full-permission-list)
    - [Permission Inheritance](#permission-inheritance)
15. [Discord Integrations — How It All Connects](#15-discord-integrations--how-it-all-connects)
    - [OAuth Login](#oauth-login)
    - [Role Syncing](#role-syncing)
    - [Discord DMs (Bot)](#discord-dms-bot)
    - [Two-Way Ticket Messaging](#two-way-ticket-messaging)
    - [Announcements to Discord Channels](#announcements-to-discord-channels)
    - [Division Discord Servers](#division-discord-servers)
    - [Roster ↔ Discord Roles](#roster--discord-roles)
16. [External Integrations](#16-external-integrations)
    - [FiveM Game Server](#fivem-game-server)
    - [Tebex Store](#tebex-store)
    - [QBCore Database](#qbcore-database)
    - [OpenAI (GPT-4o-mini)](#openai-gpt-4o-mini)
17. [Quick Reference — Common Staff Tasks](#17-quick-reference--common-staff-tasks)
18. [FAQ](#18-faq)

---

## 1. Overview

The Power Roleplay website ([powerroleplay.net](https://powerroleplay.net)) is the central hub for the entire community. It handles:

- **Authentication** — Login via Discord OAuth
- **Applications** — Whitelisted jobs, staff, and developer positions
- **Support Tickets** — Full ticketing system with Discord DM integration
- **Divisions** — Law Enforcement, Medical Services, Businesses, Real Estate, and Factions, each with rosters, ranks, and management tools
- **Staff Panel** — Administrative dashboard for managing the community
- **Power AI** — AI assistant trained on server knowledge
- **Announcements** — Send messages directly to Discord channels from the website
- **Live Stats** — Real-time FiveM player count and Discord member count
- **Rulebook** — Editable community rules
- **Help Center** — Comprehensive player guides

Everything is connected to Discord. Your website permissions come from your Discord roles, and actions like approving applications or replying to tickets automatically send Discord DMs to the relevant players.

---

## 2. Getting Started — Authentication & Login

### How Login Works

1. Go to [powerroleplay.net](https://powerroleplay.net) and click **"Sign In with Discord"** in the top-right corner
2. You'll be redirected to Discord's OAuth page — click **Authorize**
3. Discord sends your profile (username, avatar, email) back to the website
4. The website creates or updates your account and pulls your Discord roles
5. You're redirected to your [Dashboard](https://powerroleplay.net/dashboard)

### Important Details

- **There is no separate registration** — all accounts are created through Discord OAuth
- Your login session lasts **7 days** before you need to sign in again
- Your **Discord roles are synced automatically** every ~5 minutes while you're active on the site
- If an admin gives you a new Discord role, it will appear on the website within 5 minutes — no need to log out and back in
- Your **permissions are determined by your Discord roles** — the website reads your roles and looks up what permissions each role grants

### Logging Out

Click your avatar in the top-right → **Log Out**. This clears your session cookie.

---

## 3. The Homepage

**URL:** [powerroleplay.net](https://powerroleplay.net)

The homepage is public and visible to everyone, even without logging in. It features:

| Section | Description |
|---------|-------------|
| **Hero** | Full-screen rotating background slideshow (10 images, changes every 6 seconds), Power RP logo, tagline, "Get Started" and "Read Rules" buttons, Help button |
| **Built Different** | 6 feature highlight cards: Custom Framework, Active Community, Dedicated Staff, Immersive World, Easy Applications, 24/7 Support |
| **Applications** | 3 cards linking to application portal: Whitelisted Jobs, Staff Applications, Developer Applications |
| **Support** | Links to create or view support tickets |

---

## 4. Navigation Bar

The navigation bar is fixed at the top of every page and adapts based on your login status and role.

### Links (Always Visible)

| Link | Destination |
|------|-------------|
| **Home** | `/` |
| **Rules** | `/rules` |
| **Applications** | `/applications` |
| **Divisions** | Dropdown → All Divisions, Law Enforcement, Medical Services, Businesses, Real Estate, Factions |
| **Tickets** | `/tickets` |

### Right-Side Elements

| Element | Description |
|---------|-------------|
| **Player Count** | Live FiveM player count (green = online, red = offline) + Discord member count, with "Join Now" links |
| **Help Button** | Opens the Help Center modal |
| **Notification Bell** | Shows unread notification count; plays a chime sound when new notifications arrive; click to view, mark read, or clear all |
| **User Menu** | Your Discord avatar → Dashboard, Staff Panel (if staff), Log Out |

### Staff Panel Link

The **Staff Panel** link only appears if you have **any** of:
- Role: `staff` or `admin`
- Permission: `staff_access`

### Mobile

On mobile, the navbar collapses into a hamburger menu with all the same links organized vertically. The Divisions section expands inline.

---

## 5. User Dashboard

**URL:** [powerroleplay.net/dashboard](https://powerroleplay.net/dashboard)  
**Requires:** Login

Your personal dashboard showing:

- **Welcome message** with your Discord username
- **4 stat cards:** Open Tickets, Pending Applications, Approved Applications, Total Submissions
- **Quick Actions:** Create New Ticket, Submit Application
- **Recent Tickets** — Last 5 tickets with status badges
- **Recent Applications** — Last 5 applications with status badges

---

## 6. Notifications System

The notification bell in the navbar is your real-time alert system. Notifications are created automatically when:

| Event | Who Gets Notified |
|-------|-------------------|
| Application status changes (approved/denied/under review) | The applicant |
| Staff replies to your ticket | The ticket author |
| Your ticket is resolved/closed | The ticket author |
| Player replies to a ticket (or via Discord DM) | The assigned staff member |
| Auto-close reminders and closures | The ticket author |

### How It Works

- The bell polls for new notifications every **30 seconds**
- A **red badge** shows the number of unread notifications
- A **chime sound** plays when new notifications arrive (uses Web Audio API)
- Click the bell to see your last 50 notifications
- **Mark as Read** — Click the checkmark on individual notifications or "Mark All Read"
- **Clear All** — Permanently remove all notifications

---

## 7. Power AI — AI Chat Assistant

**Accessible from:** Floating button on every page (bottom-right corner)

Power AI is an AI-powered assistant that can answer questions about the server, rules, gameplay, and more. It's available to **everyone** — no login required.

### What Power AI Knows

Power AI automatically stays up to date by reading from the database every 5 minutes:

- All **rulebook sections** (the complete rules)
- All **help articles** (player guides)
- All **factions** and their member counts
- All **businesses** grouped by category
- All **real estate agencies**, zones, and property types
- All entries in the **AI Knowledge Base** (staff-managed)
- Live stats (user count, open tickets, pending applications)

### Using Power AI

1. Click the floating AI button (blue/purple gradient, bottom-right)
2. Type a question or select from the 5 suggested questions:
   - "How do I join the server?"
   - "What are the basic rules?"
   - "How do I apply for LSPD?"
   - "Tell me about the server features"
   - "How do I create a support ticket?"
3. AI responds with formatted text (bold, lists, links, code blocks)
4. Conversation is kept until you click **Clear Chat**

### Staff: Managing Power AI's Knowledge

Staff with `manage_power_ai` or `admin_access` can add, edit, and remove AI knowledge entries from the **Power AI tab** in the Staff Panel. This lets you teach the AI new information without touching code. See [Power AI Knowledge Base Tab](#power-ai-knowledge-base-tab).

### Rate Limit

- **20 messages per minute** per person (based on IP address)
- Maximum **2,000 characters** per message

---

## 8. Help Center

**Accessible from:** Help button in the navbar or on the homepage hero

The Help Center is a tabbed modal with comprehensive guides:

| Tab | Content |
|-----|---------|
| **New Player Guide** | Getting started, how to join, basic gameplay info |
| **Website Help** | How to use the website features |
| **Game Quality & Settings** | Graphics settings, performance tips, FAQ accordion |

### Staff: Editing the Help Center

Staff with `edit_help_menu` or `admin_access` see an **Edit button** on each section. Editing is done inline — update the title and content, then save. All changes are instant.

---

## 9. Rulebook

**URL:** [powerroleplay.net/rules](https://powerroleplay.net/rules)

The rulebook displays all server rules organized into sections. It features:

- **Sidebar table of contents** (sticky on desktop, slide-out on mobile) with scroll-spy highlighting
- **Severity classification system** (A–H) with color-coded badges showing punishment levels
- **Numbered rule entries** with rich formatting

### Staff: Editing Rules

Staff with `edit_rules` or `admin_access` permission see an **Edit button** on each section. Click to edit the section title and content, then save.

---

## 10. Applications System

### Application Types

There are **12 application types** organized into 3 categories:

| Category | Types |
|----------|-------|
| **Whitelisted Jobs** | BCSO (Blaine County Sheriff), LSPD, SASP, EMS, Judge, Lawyer |
| **Staff** | Staff |
| **Developer** | Web Dev, 3D Dev, LUA Dev, Graphic Design, Car Handling |

> **Note:** BCSO, LSPD, SASP, and EMS applications are managed through their respective Division pages (Law Enforcement / Medical Services), not the main staff applications page. Staff, Judge, Lawyer, and all Developer applications are managed on the Staff Panel.

### Submitting an Application

**URL:** [powerroleplay.net/applications](https://powerroleplay.net/applications)

1. Log in and go to the Applications page
2. Click on the type you want to apply for
3. Fill out the form — fields vary by type:
   - **LE/EMS/Judge/Lawyer:** Character Name, Character Backstory, RP Experience, Why Power Roleplay, Additional Info
   - **Staff:** About Yourself, Why join the staff team, Relevant Experience, Additional Info
   - **Developer:** Your Name/Alias, About You & Skills, Relevant Experience, Portfolio & Examples, Additional Info
   - Fields can be **customized by staff** per application type
4. Submit — you'll be redirected to your application page

### Important Rules

- You can only have **ONE pending/under-review application per type** at a time
- If your application shows "Already Applied," you must wait for a decision
- After being **approved or denied**, you can re-apply
- All applications are **scanned by the AI detection system** on submission (see below)

### Application Lifecycle

```
📩 Pending → 🔍 Under Review → ✅ Approved
                               → ❌ Denied
```

1. **Pending** — Submitted, waiting for staff review
2. **Under Review** — A staff member has started reviewing it
3. **Approved** — Accepted! You'll receive a Discord DM with next steps
4. **Denied** — Rejected with a reason. You can re-apply

### What Happens on Approval

| Application Type | What Happens Automatically |
|------------------|---------------------------|
| **BCSO / LSPD / SASP** | Discord DM with next steps: Join the LE Discord, request an interview |
| **EMS** | Discord DM with next steps: Join the EMS Discord, request an interview |
| **Staff** | All 5 staff Discord roles are **automatically granted**. Discord DM with welcome message, instructions to post in #needs-training |
| **All others** | Discord DM notification with approval and reviewer info |

### What Happens on Denial

- Discord DM with the denial reason and reviewer name
- In-app notification
- Player can re-apply after denial

### AI Detection System

Every application is automatically scanned for AI-generated content on submission. The system checks for:

| Signal | What It Detects |
|--------|-----------------|
| AI-typical phrases | Words like "delve," "tapestry," "multifaceted," "leverage" |
| Transition overuse | "Furthermore," "moreover," "consequently" |
| Sentence uniformity | Nearly identical sentence lengths (AI pattern) |
| Excessive formality | No contractions used at all |
| Repetitive starters | "I am a," "I believe," "My background" repeated |
| Word sophistication | Unusually high ratio of complex words |
| No informal markers | Zero typos, no slang, no emojis, no double spaces |
| Cross-field consistency | Multiple fields all flagged → bonus points |

**Scoring:**
- **0–29:** Low (probably human) — no indicator shown
- **30–59:** Medium / Suspicious — yellow **SUS** badge shown to reviewers
- **60–100:** High (likely AI) — red **AI** badge shown to reviewers

Staff see these badges when reviewing applications. The AI score is a **guide, not definitive** — always use your judgment.

### Reviewing Applications (Staff)

**URL:** [powerroleplay.net/staff/applications](https://powerroleplay.net/staff/applications)

**Required Permissions:** `manage_applications`, or type-specific `app_*` permissions (e.g., `app_staff`, `app_judge`)

1. Go to **Staff Panel → Manage Applications** (or click the tab)
2. Two category tabs:
   - **Staff Applications** (amber) — staff, judge, lawyer
   - **Developer Applications** (purple) — web_dev, dev_3d, lua_dev, graphic_dev, car_dev
3. Each tab shows pending count badge
4. Filter by status or search by name/ID/type
5. Click an application to review it

**On the review page you can:**
- Read all application fields and custom answers
- View the applicant's **Discord profile** (avatar, account age, join date, nickname, in-server status)
- See the **AI detection score** and signals
- Run a fresh **AI Check** to re-analyze
- Add **staff notes** (visible only to staff)
- **Approve** or **Deny** with an optional reason

> **Note for LE/EMS applications:** These are reviewed on the Division Applications page, not the main staff applications page. See [Division Permissions](#division-permissions).

### Customizing Application Questions

**URL:** [powerroleplay.net/staff/applications/editor](https://powerroleplay.net/staff/applications/editor) (via Staff Panel → Application Editor tab)

**Required Permissions:** `admin_access`, or type-specific `edit_app_*` (e.g., `edit_app_staff`)

You can customize the questions asked for each application type:
1. Select the application type
2. Add, remove, or reorder fields
3. Each field has: Key name, Label, Placeholder text, Required toggle, Position order
4. Maximum **20 fields** per application type
5. Save changes — they take effect immediately for new applications

---

## 11. Tickets (Support) System

### Creating a Ticket

**URL:** [powerroleplay.net/tickets/new](https://powerroleplay.net/tickets/new)

1. Log in and click **Tickets** in the navbar, then **New Ticket**
2. Fill out:
   - **Subject** — Brief description of your issue
   - **Category** — Select from the list below
   - **Priority** — Low, Normal, High, or Urgent
   - **Message** — Describe your issue in detail
3. Some categories require additional verification (see below)
4. Submit

> **Limit:** Each user can only have **ONE open ticket** at a time. You must wait for your current ticket to be resolved or closed before creating a new one.

### Ticket Categories

| Category | Description | Special Requirements |
|----------|-------------|---------------------|
| **General** | General questions and support | None |
| **Bug Report** | Report a bug or glitch | None |
| **Player Report** | Report another player | **Citizen ID verification required** — must enter the reported player's Citizen ID |
| **Appeal** | Ban or punishment appeal | None |
| **Support** | Technical support | None |
| **Purchase Inquiry** | Questions about store purchases | None |
| **Redeem Purchase** | Redeem a Tebex store purchase | **Tebex transaction ID verification required** — must enter Transaction ID (e.g., `tbx-xxx`) |
| **Other** | Anything else | None |

### Tebex Purchase Verification

When creating a **Redeem Purchase** ticket:

1. Enter your Tebex **Transaction ID** (found in your purchase confirmation email, format: `tbx-xxxxx`)
2. Click **Verify Transaction**
3. The system contacts the Tebex API and displays:
   - Amount and currency
   - Payment status and date
   - Player name
   - Payment gateway
   - Packages purchased
4. If valid, you can proceed with the ticket. Staff will see these details in the ticket sidebar.

### Citizen ID Verification

When creating a **Player Report** ticket:

1. Enter the **Citizen ID** of the player you're reporting (e.g., `ABC12345`)
2. Click **Verify Citizen**
3. The system looks up the player in the QBCore game database and shows:
   - Citizen ID and character name
   - Current job and gang
4. If valid, you can proceed. Staff will see the reported player's details in the ticket sidebar.

### Ticket Lifecycle & Statuses

```
🟢 Open → 🔵 In Progress → 🟡 Awaiting Response → ✅ Resolved
                                                   → ❌ Closed
```

| Status | Meaning |
|--------|---------|
| **Open** | New ticket, or player has replied |
| **In Progress** | Staff is actively working on it |
| **Awaiting Response** | Staff replied, waiting for the player to respond |
| **Resolved** | Issue has been resolved |
| **Closed** | Ticket is closed (by staff, player, or auto-close) |

**Automatic status changes:**
- When **staff replies** → status changes to **Awaiting Response** automatically
- When **player replies** → status changes to **Open** automatically
- When a ticket has been **Awaiting Response for 24 hours** with no reply → **Auto-Closed**

### Discord DM Integration

The ticket system is deeply integrated with Discord DMs:

| Event | What Happens |
|-------|-------------|
| **Staff replies on the website** | Player receives a Discord DM with the staff member's name, a preview of the message, and a link to the ticket |
| **Ticket is resolved/closed by staff** | Player receives a Discord DM with the status, who resolved it, and a link to the ticket |
| **Player replies via Discord DM** | The reply is automatically added to the ticket on the website. Staff get a bell notification saying "(player) replied via Discord DM" |
| **Awaiting response 6+ hours** | Player gets a reminder DM saying their ticket will auto-close |
| **Auto-closed (24h no response)** | Player gets a red Discord DM saying the ticket was closed due to no response |

### Two-Way DM Messaging

When staff replies to a ticket on the website, the player gets a DM. If the player replies to that DM in Discord, the message is automatically relayed back to the ticket on the website. This means **players can respond to tickets entirely from Discord** without needing to visit the website.

### Auto-Close System

The auto-close worker runs continuously (every 5 minutes):

1. **6-hour mark:** If a ticket has been in "Awaiting Response" for 6+ hours, a warning DM is sent to the player reminding them to respond. This repeats every 6 hours.
2. **24-hour mark:** If the player still hasn't responded after 24 hours, the ticket is automatically closed and a final DM is sent.

### Managing Tickets (Staff)

**URL:** [powerroleplay.net/staff/tickets](https://powerroleplay.net/staff/tickets)

**Required Permissions:** `manage_tickets` (all categories), or category-specific permissions like `ticket_general`, `ticket_player_report`, etc.

#### Category Overview

The staff ticket page shows a grid of all ticket categories you have access to. Each category card displays:
- Total ticket count
- Active tickets (open + in-progress + awaiting)
- Color-coded mini status bar

Click a category to drill into it.

#### Category Detail View

- **Status filter** buttons with counts (Open, In Progress, Awaiting, Resolved, Closed)
- **Search** by subject, author name, or ticket ID
- Click a ticket to open the full detail view

#### Staff Ticket Detail View

**URL:** [powerroleplay.net/staff/tickets/{id}](https://powerroleplay.net/staff/tickets/)

A 2-column layout with the message thread on the left and a rich sidebar on the right:

**Message Thread (Left):**
- Full chat history (staff messages highlighted in blue with a "Staff" badge)
- Real-time polling every 10 seconds for new messages
- Reply input at the bottom

**Sidebar (Right):**

| Panel | Description |
|-------|-------------|
| **Actions** | Change status (dropdown), change priority, Quick Resolve/Close buttons |
| **Details** | Category, author info, dates, assigned staff |
| **Tebex Purchase** | (Redeem Purchase tickets only) Full transaction details, packages, refund status |
| **Reported Player** | (Player Report tickets only) Citizen ID, character name, job, gang — live from game DB |
| **AI Assist** | Click "Summarize with AI" — generates a summary + 3 suggested responses. Click "Use" to paste a suggestion into the reply box |
| **Discord Profile** | Applicant's Discord avatar, banner, username, ID, account age, server join date, nickname, roles, "NOT IN SERVER" warning if they've left |

### AI Ticket Assistant

The AI Assist feature uses **GPT-4o-mini** to help staff handle tickets faster:

1. Click **"Summarize with AI"** in the ticket sidebar
2. The AI reads the full ticket conversation and generates:
   - **Summary:** What the issue is, key details, current status, recommended next steps, any red flags
   - **3 Suggested Responses:** Different approaches — e.g., ask for more info, resolve the issue, cite a rule
3. Click **"Use"** on any suggestion to paste it into your reply box
4. Edit the suggestion as needed, then send

---

## 12. Divisions System

**URL:** [powerroleplay.net/divisions](https://powerroleplay.net/divisions)

Power Roleplay has 5 divisions, each with its own Discord server, roster system, and management tools:

| Division | Discord Server | Departments |
|----------|---------------|-------------|
| **Law Enforcement** | LE Discord | SACO, LSPD, BCSO, GIU, SASP |
| **Medical Services** | EMS Discord | EMS |
| **Businesses** | Businesses Discord | Management, Operations |
| **Real Estate** | Real Estate Discord | Sales & Leasing, Development |
| **Factions** | Factions Discord | Gangs, Mafias |

### Division Landing Pages

Each division has a public landing page (`/divisions/{slug}`) showing:
- Hero image with stats
- About section
- Department cards with "Apply Now" buttons (or "Internal Transfer Only" for some departments)
- **Public Chain of Command** — a rank pyramid showing leadership, visible to everyone without login

### Law Enforcement

**URL:** [powerroleplay.net/divisions/law-enforcement](https://powerroleplay.net/divisions/law-enforcement)

**Departments:** SACO, LSPD, BCSO, GIU, SASP

**Features:**
- Apply for BCSO, LSPD, SASP through the Application system (SACO and GIU are internal-transfer-only)
- Roster management with drag-and-drop rank changes
- Clock-in activity tracking — hours logged from in-game duty synced to leaderboard
- Staff with LE division permissions can review LE applications directly from the division page

### Medical Services (EMS)

**URL:** [powerroleplay.net/divisions/medical-services](https://powerroleplay.net/divisions/medical-services)

**Department:** EMS

**Features:**
- Apply for EMS through the Application system
- Roster management
- Clock-in activity tracking
- EMS division application review

### Businesses

**URL:** [powerroleplay.net/divisions/businesses](https://powerroleplay.net/divisions/businesses)

**Features:**
- Browse all approved businesses
- Business owners can manage their business page (roster, ranks, applications, images)
- Apply to join a specific business
- Business rating system
- **Start a Business** — links to Tebex store to purchase a business slot
- Business reports — a ticket-like system within the division
- **Admin Business Management** — create, edit, approve/deny businesses, manage categories and statuses
- Audit log of all business changes

### Real Estate

**URL:** [powerroleplay.net/divisions/real-estate](https://powerroleplay.net/divisions/real-estate)

**Features:**
- Browse real estate agencies
- Book appointments for property viewings
- Agency dashboard for agency members (manage appointments)
- **DRE Admin Panel** — comprehensive admin interface for managing:
  - Zones and zone assignments
  - Property categories and types
  - Agencies (create, edit, assign zones/categories)
  - Pricing configurations
  - DRE staff with granular permissions
  - Agency owners and members
- Division report/ticket system

### Factions

**URL:** [powerroleplay.net/divisions/factions](https://powerroleplay.net/divisions/factions)

**Features:**
- Browse all factions
- View faction details and member lists
- **Faction leadership** is determined by Discord roles — you must have BOTH:
  1. The faction's specific Discord role (e.g., "Ballas")
  2. The `verified gang leader` or `verified co leader` role
- Leaders can manage their faction roster (add members, change ranks, remove members)
- Upload faction images
- **Start a Faction** — links to Tebex store

### Roster Management

**URL:** `/divisions/{slug}/roster`  
**Requires:** Authentication + department access (view or manage)

The roster system is the backbone of division management. It shows all members organized by rank within each department.

#### Viewing the Roster

- Members are organized by rank in a tiered display:
  - 🟡 **Command** ranks (gold styling)
  - 🔵 **Officer** ranks (blue styling)
  - ⚪ **Enlisted** ranks (grey styling)
- Each member shows their Discord avatar, display name, and username
- Switch between departments using tabs
- Search members by name

#### Managing the Roster (requires manage permission)

- **Drag & Drop** — Drag a member to a different rank to promote/demote them. The website automatically updates their Discord roles in real-time.
- **Remove** — Remove a member from the division (strips all division-specific Discord roles)
- **Terminate** — Strip ALL roles from the member across the entire Discord guild. A Discord DM is sent to the terminated member notifying them.

#### Roster Configuration

Roster configuration maps Discord roles to ranks and departments:

1. Go to **Config** panel on the roster page
2. For each department, define:
   - **Rank name** (e.g., "Captain," "Officer")
   - **Discord Role ID** — which Discord role corresponds to this rank
   - **Position** — rank order (1 = highest)
3. Save — members who have that Discord role will appear in that rank

#### Roster Permissions Setup

1. Go to **Permissions** panel on the roster page (requires `manage_division_*` or admin)
2. Map Discord roles to department access levels:
   - **None** — no roster access
   - **View** — can see the roster but not make changes
   - **Manage** — can drag-and-drop, remove, and terminate members
3. You can set access per individual department or use **All Departments** for blanket access

### Clock-In / Activity Tracking

**URL:** `/divisions/{slug}/activity` (Law Enforcement and Medical Services only)  
**Requires:** Roster access

The activity page shows a leaderboard of duty hours logged in-game:

- **Date range picker** — 7 days, 30 days, 90 days, or all time
- **Department filter** — filter by specific department (e.g., LSPD, BCSO)
- **Stats bar** — Active Members, Total Hours, Average Hours/Person
- **Leaderboard table** — sorted by hours with 🥇🥈🥉 for top 3

**How it works:**
1. When a player goes on duty in-game (FiveM), the game server sends a clock-in event to the website
2. When they go off duty or disconnect, a clock-out event is sent
3. The website tracks total hours per member
4. Data is displayed on the activity page enriched with Discord member info

### Division Permissions

Division permissions control who can manage what within each division.

#### Department Permissions (Roster Access)

| Level | Ability |
|-------|---------|
| **None** | Cannot see the roster |
| **View** | Can see the roster but cannot make changes |
| **Manage** | Full roster control (drag-and-drop, remove, terminate) |

Set up at: `/divisions/{slug}/manage` → **Roster Permissions** tab. Map Discord roles to access levels per department.

#### Application Permissions (Division-Level)

Control who can review and edit applications for department-specific types (BCSO, LSPD, SASP, EMS):

| Permission | Ability |
|------------|---------|
| **Can Review** | View and approve/deny applications for this type |
| **Can Edit** | Modify application questions for this type (auto-includes review) |

Set up at: `/divisions/{slug}/manage` → **Application Permissions** tab.

---

## 13. Staff Panel

**URL:** [powerroleplay.net/staff](https://powerroleplay.net/staff)  
**Requires:** `staff_access` permission (or admin)

The Staff Panel is the central hub for all staff operations. It has **9 tabs**, each requiring specific permissions.

### Staff Dashboard Tab

**Permission:** `staff_access`

Your staff home screen showing:

- **Stat cards** — Open Tickets, Total Tickets, Pending Applications, Total Applications (you only see stats for areas you have permission to access)
- **Quick Navigation** — Cards linking to Support Tickets, Manage Applications, Manage Permissions, Application Editor
- **Recent Items** — Last 5 tickets and 5 applications at a glance

### Support Tickets Tab

**Permission:** `manage_tickets` or any `ticket_*` permission  
**Redirects to:** `/staff/tickets`

See [Managing Tickets (Staff)](#managing-tickets-staff) for full details.

### Manage Applications Tab

**Permission:** `manage_applications` or any `app_*` permission  
**Redirects to:** `/staff/applications`

See [Reviewing Applications (Staff)](#reviewing-applications-staff) for full details.

### Manage Permissions Tab

**Permission:** `admin_access` only  
**Redirects to:** `/staff/roles`

This is where you connect Discord roles to website permissions.

#### How to Set Up Permissions

1. Click **"Sync Discord Roles"** to pull all roles from the main Discord server
2. You'll see a list of all Discord roles. Search/filter as needed.
3. Click a role to expand its permission editor
4. Check the boxes for each permission you want to grant to that Discord role
5. Changes save automatically on each toggle

#### What You See

- **Total Discord Roles** — how many roles are synced
- **Configured Roles** — how many roles have at least 1 permission
- **Staff Roles** — roles with `staff_access`
- **Admin Roles** — roles with `admin_access`

Each role shows:
- Role name with color dot
- Number of permissions granted
- "Admin" or "Staff" badge if applicable
- Expandable permission checkboxes organized by category

> **Important:** LE/EMS application permissions (BCSO, LSPD, SASP, EMS) are NOT managed here. They are managed on each division's management page because they use Discord-role-to-department mapping. Staff Panel permissions only cover Staff, Judge, Lawyer, and Developer app types.

### Application Editor Tab

**Permission:** `admin_access` or any `edit_app_*` permission  
**Redirects to:** `/staff/applications/editor`

See [Customizing Application Questions](#customizing-application-questions) for full details.

### Staff Activity / Leaderboard Tab

**Permission:** `staff_access`

A comprehensive leaderboard ranking all staff members by their activity.

**Ranking criteria (in order of priority):**
1. **Tickets Resolved** — number of tickets this staff member has resolved
2. **In-Game Duty Time** — hours spent on admin duty in-game (synced from FiveM)
3. **Web Ticket Support Time** — time spent actively viewing tickets on the website

**Leaderboard Display:**
- **Top 3 podium** — gold, silver, bronze with large cards
- All staff cards showing:
  - Discord avatar and username
  - Role (Administrator / Staff Member)
  - Top 5 Discord roles (color-coded pills)
  - Tickets Resolved count
  - In-Game Duty time
  - Web Tickets time

**How Web Ticket Time is Tracked:**
- While you're on any staff ticket page, the website sends a "heartbeat" every 60 seconds
- This accumulates your web support time automatically
- Time is tracked per day and aggregated for the leaderboard

### Staff Handbook Tab

**Permission:** `staff_access` (view), `edit_handbook` or `admin_access` (edit)

The handbook contains 7 sections that every staff member should read:

| Section | Content |
|---------|---------|
| **Welcome to the Team** | Introduction and overview of staff expectations |
| **Ranks & Responsibilities** | Trial Mod, Moderator, Senior Mod, Administrator, Head Admin — each with duties and TxAdmin permissions |
| **Staff Rules** | 6 categories of staff conduct rules with punishments |
| **Additional Staff Info** | Player clip requirements, kick/ban/warning procedures |
| **Commands Reference** | In-game admin commands, Discord commands, Donation support commands |
| **Permissions by Rank** | Table showing which TxAdmin permissions each rank gets |
| **Staff Teams** | 9 staff teams: Ban Appeal, PWR Development, Business Management, Faction Management, Reimbursement, Donation Support, Bug Control, Community Outreach, Player Report |

**Editing** (for users with `edit_handbook` or admin):
- Click any section → Edit button
- Modify title and content (JSON format)
- Save with validation

### Power AI Knowledge Base Tab

**Permission:** `manage_power_ai` or `admin_access`

This tab lets you manage what Power AI knows. Every entry you add here is automatically included in Power AI's knowledge when answering player questions.

#### Managing Entries

**Stats Dashboard:** Shows total entries, active, disabled, and number of categories used.

**Adding an Entry:**
1. Click **"Add Entry"**
2. Select a **Category** (10 defaults: General, Gameplay, Jobs & Economy, Vehicles, Housing, Criminal RP, Police/EMS, Server Info, Commands, FAQ)
3. Enter a **Title** (what the entry is about)
4. Enter the **Content** (the actual information Power AI should know)
5. Save

**Entry List:**
- Each entry shows: category badge, enabled/disabled status, title, content preview, who last edited it and when
- **Search** by title or content
- **Filter** by category
- **Actions:** Toggle enable/disable, edit, delete

**Tips:**
- Be specific and factual in entries
- Use natural language — the AI incorporates this text directly into its context
- Disabled entries are NOT included in AI responses
- Changes take effect within 5 minutes (the AI context refreshes every 5 minutes)

### Send Announcement Tab

**Permission:** `send_announcements` or `admin_access`

Send messages directly to any Discord channel in any of Power Roleplay's Discord servers, all from the website.

#### How to Send an Announcement

1. **Select a Server** — Choose from: Power Roleplay (Main), Law Enforcement, Medical Services, Businesses, Real Estate, Factions
2. **Select a Channel** — Channels are grouped by category from the Discord server
3. Choose **Message Mode:**
   - **Embed** — Rich embed with colored sidebar, heading, and up to 4,096 characters
   - **Plain Text** — Standard Discord message with up to 2,000 characters
4. (Embed mode) Set a **Heading** and choose an **Embed Color** (9 presets: Blue, Green, Red, Yellow, Purple, Pink, Cyan, Orange, White — or custom color picker)
5. Write your **Message** using the formatting toolbar
6. (Optional) Attach an **Image** — upload a file (drag & drop, max 8MB) or paste an image URL
7. (Optional) Toggle **@everyone** to ping everyone in the channel
8. (Optional) Click **"Enhance with AI"** to have GPT-4o-mini rewrite your message professionally
9. Click **Send**

#### Formatting Toolbar

The toolbar inserts Discord markdown around your selected text or at your cursor:

| Button | Markdown | Result |
|--------|----------|--------|
| H1 | `# text` | Large heading |
| H2 | `## text` | Medium heading |
| H3 | `### text` | Small heading |
| **B** | `**text**` | **Bold** |
| *I* | `*text*` | *Italic* |
| ~~S~~ | `~~text~~` | ~~Strikethrough~~ |
| `<>` | `` `text` `` | `Inline Code` |
| Code | ` ```text``` ` | Code block |
| Quote | `> text` | Block quote |
| List | `• text` | Bullet list |
| Link | `[text](url)` | Hyperlink |
| Line | `───` | Divider line |

#### Enhance with AI

The **"Enhance with AI"** button sends your draft message to GPT-4o-mini, which rewrites it to be:
- Professional and well-organized
- Properly formatted for Discord (headings, bold, bullets, separators)
- Approachable in tone
- Structured with clear sections

The enhanced message replaces your draft. You can further edit it before sending.

#### Live Preview

A real-time preview on the right side shows exactly how your message will look in Discord, including:
- Bot avatar and name
- @everyone mention (if toggled)
- Embed with colored sidebar, heading, and message (embed mode)
- Plain text with markdown rendering (plain mode)
- Image preview
- Timestamp

---

## 14. Permissions System — Complete Reference

### How Permissions Work

1. **Discord roles are the source of truth.** Your permissions on the website are determined by which Discord roles you have in the main Power Roleplay Discord server.

2. **Admins map Discord roles to permissions** on the Manage Permissions page (Staff Panel → Manage Permissions). For example, the "Senior Moderator" Discord role might be given `staff_access`, `manage_tickets`, and `manage_applications`.

3. **Roles are synced automatically.** Every ~5 minutes while you're active on the site, the website pulls your latest Discord roles and recalculates your permissions. No logout needed.

4. **Inheritance:** Some permissions automatically include others (see below).

### Full Permission List

#### Core Access
| Permission | Description |
|-----------|-------------|
| `staff_access` | Access to the Staff Panel, dashboard, activity leaderboard, handbook |
| `admin_access` | **Full access to everything** — automatically grants every other permission |

#### Ticket Management
| Permission | Description |
|-----------|-------------|
| `manage_tickets` | Access to ALL ticket categories |
| `ticket_general` | Access to General tickets only |
| `ticket_bug_report` | Access to Bug Report tickets only |
| `ticket_player_report` | Access to Player Report tickets only |
| `ticket_appeal` | Access to Appeal tickets only |
| `ticket_support` | Access to Support tickets only |
| `ticket_other` | Access to Other tickets only |
| `ticket_purchase_inquiry` | Access to Purchase Inquiry tickets only |
| `ticket_redeem_purchase` | Access to Redeem Purchase tickets only |

#### Application Review
| Permission | Description |
|-----------|-------------|
| `manage_applications` | Review ALL application types |
| `app_bcso` | Review BCSO applications |
| `app_lspd` | Review LSPD applications |
| `app_sasp` | Review SASP applications |
| `app_ems` | Review EMS applications |
| `app_judge` | Review Judge applications |
| `app_lawyer` | Review Lawyer applications |
| `app_staff` | Review Staff applications |
| `app_web_dev` | Review Web Dev applications |
| `app_dev_3d` | Review 3D Dev applications |
| `app_lua_dev` | Review LUA Dev applications |
| `app_graphic_dev` | Review Graphic Design applications |
| `app_car_dev` | Review Car Handling applications |

#### Application Editing
| Permission | Description |
|-----------|-------------|
| `edit_app_bcso` | Edit BCSO application questions |
| `edit_app_lspd` | Edit LSPD application questions |
| `edit_app_sasp` | Edit SASP application questions |
| `edit_app_ems` | Edit EMS application questions |
| `edit_app_judge` | Edit Judge application questions |
| `edit_app_lawyer` | Edit Lawyer application questions |
| `edit_app_staff` | Edit Staff application questions |
| `edit_app_web_dev` | Edit Web Dev application questions |
| `edit_app_dev_3d` | Edit 3D Dev application questions |
| `edit_app_lua_dev` | Edit LUA Dev application questions |
| `edit_app_graphic_dev` | Edit Graphic Design application questions |
| `edit_app_car_dev` | Edit Car Handling application questions |

#### Content Management
| Permission | Description |
|-----------|-------------|
| `edit_rules` | Edit the community rulebook |
| `edit_handbook` | Edit the staff handbook |
| `edit_help_menu` | Edit the Help Center content |
| `manage_power_ai` | Manage Power AI knowledge base entries |
| `manage_users` | User management |

#### Announcements
| Permission | Description |
|-----------|-------------|
| `send_announcements` | Send announcements to Discord channels |

#### Division Management
| Permission | Description |
|-----------|-------------|
| `manage_division_le` | Manage Law Enforcement division permissions, config, and roster |
| `manage_division_med` | Manage Medical Services division permissions, config, and roster |
| `manage_division_biz` | Manage Businesses division permissions, config, and roster |
| `manage_division_re` | Manage Real Estate division permissions, config, and roster |
| `manage_division_fac` | Manage Factions division permissions, config, and roster |

### Permission Inheritance

Some permissions automatically include others:

| If You Have | You Also Get |
|------------|-------------|
| `admin_access` | **Every single permission** |
| `manage_tickets` | All `ticket_*` category permissions |
| `manage_applications` | All `app_*` type permissions |

---

## 15. Discord Integrations — How It All Connects

The website is deeply integrated with Discord at every level. Here's how each integration works:

### OAuth Login

- Players authenticate by clicking "Sign In with Discord"
- The website uses Discord OAuth2 with the `identify` and `email` scopes
- After authorization, the website receives the player's Discord ID, username, avatar, and email
- This creates or updates their website account

### Role Syncing

**How it works:**
1. When a user logs in, the website calls the Discord API (using the bot token) to fetch all their roles in the main Power Roleplay guild
2. Roles are stored in the `user_discord_roles` table
3. Every 5 minutes while the user is active, their roles are re-synced
4. The website looks up what permissions are mapped to each Discord role (via the Manage Permissions page)
5. The user's permissions are recalculated

**For division Discord servers:**
- Division pages also sync roles from the division-specific Discord servers
- Example: When viewing the LE division page, your roles from the LE Discord server are synced too
- This is how roster membership and division-level permissions work

### Discord DMs (Bot)

The Power Roleplay Discord bot sends DMs to players for:

| Event | DM Content |
|-------|-----------|
| Application approved | Congratulations message + next steps (LE: join LE Discord + interview; EMS: join EMS Discord + interview; Staff: welcome + training instructions) |
| Application denied | Denial notification with reason |
| Application under review | Status update notification |
| Staff replies to ticket | Message preview + link to ticket |
| Ticket resolved/closed | Status notification + link |
| Ticket awaiting response (6h) | Reminder to respond or ticket will auto-close |
| Ticket auto-closed (24h) | Closure notification |
| Member terminated from roster | Notification that all roles were removed |

All DMs include rich embeds with:
- Color coding (amber = pending, blue = review, green = approved, red = denied)
- Application/ticket details
- Links back to the website
- "Power Roleplay — powerroleplay.net" footer

### Two-Way Ticket Messaging

This is one of the most powerful integrations:

1. Staff replies to a ticket on the website → player gets a DM
2. Player replies to that DM in Discord → the message is automatically relayed into the ticket on the website
3. Staff gets a bell notification that the player replied (via Discord DM)
4. This loop continues — players never need to visit the website to respond to tickets

**Technical flow:**
- The website runs a Discord WebSocket Gateway listener (embedded in the Next.js server via `instrumentation.ts`)
- This listener watches for DMs sent to the bot
- When it detects a DM reply, it calls the internal `/api/tickets/discord-reply` endpoint
- That endpoint matches the DM to the correct open ticket and inserts the message

### Announcements to Discord Channels

From the Staff Panel → Send Announcement tab, staff can send messages to any text channel in any configured Discord server:

- **Power Roleplay (Main)** — Guild ID from `DISCORD_GUILD_ID`
- **Law Enforcement** — Guild ID from `DIVISION_LE_GUILD_ID`
- **Medical Services** — Guild ID from `DIVISION_MED_GUILD_ID`
- **Businesses** — Guild ID from `DIVISION_BIZ_GUILD_ID`
- **Real Estate** — Guild ID from `DIVISION_RE_GUILD_ID`
- **Factions** — Guild ID from `DIVISION_FAC_GUILD_ID`

The message is sent via the Discord Bot API as if the bot posted it. It can include embeds, images, and @everyone pings.

### Division Discord Servers

Each division has its own Discord server. The website connects to these servers to:

- Fetch member lists for rosters
- Read and assign Discord roles for rank management
- Drag-and-drop rank changes on the website automatically update the member's Discord roles in real-time
- Terminating a member from the roster strips all their roles in the division Discord

### Roster ↔ Discord Roles

The roster system works by mapping Discord roles to ranks:

1. Admin configures: "Discord Role X = Captain rank in LSPD department"  
2. The website fetches all members from the division's Discord server
3. Members who have Role X appear as Captains in the LSPD roster
4. When you drag a member from Captain to Sergeant on the website, the website:
   - Removes the Captain Discord role from them
   - Adds the Sergeant Discord role to them
   - All via the Discord API in real-time

---

## 16. External Integrations

### FiveM Game Server

The website connects to the FiveM game server in two ways:

1. **Server Status** — Queries the FiveM `dynamic.json` endpoint every 15 seconds to show live player count
2. **Clock-In Data** — The game server sends duty clock-in/clock-out events to `/api/clockin` when staff or officers go on/off duty
3. **Staff In-Game Data** — The game server periodically syncs staff duty hours, XP, and steam IDs to `/api/staff/activity/ingame`

**FiveM Connect URL:** [cfx.re/join/opvd97](https://cfx.re/join/opvd97)

### Tebex Store

The Tebex integration lets staff verify purchase transactions when players submit Redeem Purchase tickets:

- Players enter their Tebex Transaction ID (format: `tbx-xxxxx`)
- The website calls the Tebex Payments API to verify the transaction
- Returns: amount, date, status, currency, payment gateway, packages purchased, player info
- Staff see these details in the ticket sidebar to help process redemption requests

### QBCore Database

The QBCore database integration lets staff look up player data from the game:

- Used when creating Player Report tickets — player enters a Citizen ID to identify the reported player
- The website queries the QBCore MySQL database directly
- Returns: citizen ID, character name, Steam name, license, current job, gang affiliation
- Staff see this in the ticket sidebar to help investigate player reports

### OpenAI (GPT-4o-mini)

OpenAI's GPT-4o-mini model powers three features:

1. **Power AI Chat** — The public AI assistant on every page
2. **AI Ticket Assistant** — Staff tool for summarizing tickets and generating response suggestions
3. **AI Announcement Enhancement** — Rewrites announcement drafts to be more professional
4. **AI Detection** — Analyzes application text for AI-generated content patterns (this is a local heuristic system, not OpenAI-powered)

---

## 17. Quick Reference — Common Staff Tasks

### Review an Application

1. Staff Panel → **Manage Applications** tab
2. Click the application you want to review
3. Read the answers, check the AI score, view the applicant's Discord profile
4. Click **Approve** or **Deny**, add a reason if denying
5. The applicant automatically receives a Discord DM

### Handle a Support Ticket

1. Staff Panel → **Support Tickets** tab → click a category → click a ticket
2. Read the conversation, check sidebar panels (Tebex data, reported player info, Discord profile)
3. Use **AI Assist** to get a summary and suggested responses if needed
4. Type your reply and click **Send** (status auto-changes to "Awaiting Response")
5. The player receives a Discord DM with your message

### Add Someone to a Division Roster

1. Go to `/divisions/{slug}/roster`
2. They must already have the correct Discord role in the division's Discord server
3. The website will automatically show them in the roster based on their roles

### Promote/Demote a Division Member

1. Go to `/divisions/{slug}/roster`
2. Find the member
3. **Drag and drop** them to the new rank
4. Their Discord roles are updated automatically

### Remove/Terminate a Division Member

1. Go to `/divisions/{slug}/roster`
2. Find the member
3. Click the **⋮** menu
4. Choose **Remove** (strips division roles only) or **Terminate** (strips ALL roles + sends DM)

### Send a Discord Announcement

1. Staff Panel → **Send Announcement** tab
2. Select server and channel
3. Choose Embed or Plain Text mode
4. Write your message (use the formatting toolbar)
5. Optionally use "Enhance with AI" to polish it
6. Click **Send**

### Sync Discord Roles

1. Staff Panel → **Manage Permissions** tab
2. Click **"Sync Discord Roles"**
3. Wait for the sync to complete
4. You'll see all Discord roles updated

### Grant Staff Permissions to a Role

1. Staff Panel → **Manage Permissions** tab
2. Find the Discord role (search by name)
3. Click to expand
4. Check/uncheck permission boxes
5. Changes save automatically

### Add Power AI Knowledge

1. Staff Panel → **Power AI** tab
2. Click **"Add Entry"**
3. Choose a category, enter title and content
4. Save — Power AI will use this knowledge within 5 minutes

### Edit the Rulebook

1. Go to [powerroleplay.net/rules](https://powerroleplay.net/rules)
2. Click **Edit** on the section you want to change
3. Modify the title or content
4. Click **Save**

### Edit the Help Center

1. Click the **Help** button in the navbar
2. Navigate to the section you want to edit
3. Click the **Edit** button (visible if you have `edit_help_menu` permission)
4. Make your changes and save

---

## 18. FAQ

### General

**Q: How do I access the Staff Panel?**  
A: You need the `staff_access` permission, which is granted via a Discord role. If you have a Staff role in Discord, it should work. If not, ask an admin to check your role permissions on the Manage Permissions page.

**Q: I was given a new Discord role but my permissions haven't updated. What do I do?**  
A: Wait up to 5 minutes — the website syncs your Discord roles automatically. If it still doesn't work, try logging out and back in to force a full re-sync.

**Q: Can players see staff notes on applications?**  
A: Players can see the `staff_notes` and `review_reason` fields. However, they cannot see AI detection scores or signals — those are staff-only.

**Q: Can I have multiple Discord roles granting permissions?**  
A: Yes! Permissions are additive. If Role A gives you `ticket_general` and Role B gives you `ticket_appeal`, you'll have access to both General and Appeal tickets.

### Applications

**Q: Why can't I see LE/EMS applications in the Manage Applications tab?**  
A: BCSO, LSPD, SASP, and EMS applications are managed through their respective Division pages. In the Staff Panel → Manage Applications, the scope filter (`scope=staff_panel`) specifically excludes these types. Go to `/divisions/law-enforcement` or `/divisions/medical-services` and click "View Applications" instead.

**Q: How does the AI detection work? Is it accurate?**  
A: The AI detection uses a heuristic scoring system that checks for patterns common in AI-generated text (overly formal language, certain vocabulary, uniform sentence structure, etc.). It scores 0–100. Scores below 30 are probably human; 30–59 are suspicious; 60+ are likely AI. It's a guide, not a guarantee — always review applications with your own judgment.

**Q: What happens when I approve a staff application?**  
A: Three things happen automatically: (1) The applicant gets 5 staff Discord roles added to them, (2) They get a Discord DM welcoming them with instructions to post in #needs-training, (3) An in-app notification is created. If the applicant is NOT in the Discord server, the approval will fail with an error telling you to have them rejoin first.

### Tickets

**Q: What is the auto-close system?**  
A: When staff replies to a ticket, it enters "Awaiting Response" status. If the player doesn't respond within 6 hours, they get a reminder DM. If they still don't respond after 24 hours total, the ticket automatically closes and they get a notification.

**Q: How does two-way Discord DM messaging work?**  
A: When you reply to a ticket on the website, the player gets a DM. If they reply to that DM in Discord, their message is automatically inserted into the ticket on the website, and you get a bell notification. This means players can use tickets entirely from Discord.

**Q: Can a player have multiple tickets open?**  
A: No. Each player can only have one open ticket at a time. They must wait for their current ticket to be resolved or closed before creating a new one.

### Divisions

**Q: How do roster ranks work?**  
A: Each rank in a department is mapped to a specific Discord role. When a member has that Discord role, they appear at that rank in the roster. Changing a member's rank via drag-and-drop on the website automatically adds/removes the corresponding Discord roles.

**Q: What's the difference between Remove and Terminate?**  
A: **Remove** strips only the division-specific Discord roles (the roles mapped to ranks in that division). **Terminate** strips ALL roles from the member in the entire Discord guild and sends them a DM notification. Use Terminate for disciplinary actions.

**Q: Why can't I see a member in the roster?**  
A: They might not have any Discord roles that are mapped to ranks. Check the Roster Config to make sure their Discord role is mapped to a department and rank.

### Announcements

**Q: What's the difference between Embed and Plain Text mode?**  
A: **Embed** mode sends a rich embed with a colored sidebar, heading text, and up to 4,096 characters. **Plain Text** mode sends a regular Discord message with markdown formatting and up to 2,000 characters. Embeds look more professional and stand out more.

**Q: What does "Enhance with AI" do?**  
A: It sends your draft message to GPT-4o-mini, which rewrites it to be more professional, organized, and properly formatted for Discord. It keeps the same information but improves the presentation. You can further edit the result before sending.

**Q: Can I send images in announcements?**  
A: Yes! You can either upload an image file (max 8MB, PNG/JPG/GIF/WEBP) using drag-and-drop, or paste an image URL. The image will appear in the Discord message.

### Permissions

**Q: I'm an admin but where do I set LE/EMS application permissions?**  
A: LE and EMS application permissions (who can review BCSO, LSPD, SASP, EMS applications) are set on the division management page, not the main Manage Permissions page. Go to `/divisions/law-enforcement/manage` → **Application Permissions** tab.

**Q: What does `admin_access` do?**  
A: It grants **every single permission** on the website. If a Discord role has `admin_access`, anyone with that role can do everything — manage all tickets, all applications, all divisions, all content, and see the full Manage Permissions page.

---

> **Still have questions?** Create a support ticket at [powerroleplay.net/tickets/new](https://powerroleplay.net/tickets/new) or ask in the Discord staff channels.
>
> *This documentation is maintained by the Power Roleplay development team. If you notice anything outdated or incorrect, please let an admin know.*
