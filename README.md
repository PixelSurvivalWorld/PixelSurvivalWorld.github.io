# Pixel Survival World - Website Design Document

## Overview

"Pixel Survival World" is a game that combines pixel art style, survival gameplay, and blockchain technology. The official website design adopts a cartoonish, pixel art style similar to Minecraft's aesthetics, while showcasing the game's core features and blockchain-enabled innovations.

## Design Style

- **Pixel Art Style**: All UI elements, buttons, and icons use pixel art treatment
- **Color Scheme**: Bright, saturated colors with green (representing survival) and blue (representing blockchain technology) as primary colors
- **Typography**: Pixel-style fonts that maintain readability while staying consistent with the game style
- **Animations**: Simple but engaging pixel animations for hover effects, loading states, etc.

## Website Structure and Pages

### 1. Home Page

#### Top Navigation Bar
- Game Logo (pixel style)
- Navigation Links: Home, Game Intro, Features, NFT Market, Community, Download
- Connect Wallet Button (prominent position)
- Language Switcher

#### Hero Section
- Full-screen pixel-style game scene background
- Prominent Title: "Pixel Survival World"
- Subtitle: "Blockchain-Powered Survival Adventure"
- Main Action Buttons:
  - "Play Now"
  - "Connect Wallet"
  - "Learn More"
- Brief game introduction animation (short clip of pixel characters in the survival world)

#### Game Highlights Overview
- 3-4 icons and brief descriptions of core features:
  - Survival Play
  - Blockchain Integration
  - Pixel Building
  - Community Creation

#### Latest Announcements/News
- Scrolls to display latest game updates, events, and community news
- Each contains date, title, and brief description
- "View All" button

#### Game Trailer
- Embedded video player to showcase game trailer
- Pixel-style video control buttons

#### Community Data Display
- Player Count
- Created World Count
- Transaction Data on Blockchain
- Use pixel-style counters and icons

### 2. Game Introduction Page

#### Game Story
- Pixel-style story illustrations
- Game background story text
- Displayed in chapters

#### Game World
- Display of different biosphere systems
- Pixel-style world map
- Brief description of each area

#### Game Characters
- Display of selectable characters
- Character features and abilities description
- Pixel-style character illustrations

#### Game Objectives
- Survival mechanism description
- Game progress and achievement system
- Use pixel icons to describe different objectives

### 3. Game Features Page

#### Survival Play
- Resource collection system
- Building mechanism
- Survival challenges
- Use pixel-style explanatory diagrams

#### Blockchain Integration
- Token economy description
- Digital ownership concept
- Blockchain technology advantages
- Use simplified pixel-style charts

#### Game NFTs
- NFT item display
- Rarity system
- Collection value
- Pixel-style NFT display frame

#### Community Governance
- DAO mechanism description
- Voting system
- Community proposal process
- Pixel-style governance icons

### 4. NFT Market Page

#### Market Overview
- Popular NFT display
- Price trend
- Transaction volume data
- Pixel-style charts and data visualization

#### Browse Categories
- By type (weapons, equipment, land, etc.)
- By rarity
- By price
- Pixel-style category icons

#### NFT Details
- Large image display
- Attribute list
- Transaction history
- Current owner
- Bid/Purchase button

#### My Collection
- Displayed NFTs I own
- Sale management
- Pixel-style collection display frame

### 5. Community Page

#### Announcement Board
- Official announcements
- Update log
- Activity calendar
- Pixel-style announcement board design

#### Player Display
- Excellent player works
- Community creation content
- Player ranking
- Pixel-style display frame

#### Forum Entry
- Latest hot topics
- Category discussion area
- Pixel-style forum icons

#### Social Media
- Social media links
- Discord server invitation
- Pixel-style social media icons

### 6. Download Page

#### System Requirements
- Minimum configuration
- Recommended configuration
- Pixel-style computer/device icons

#### Download Options
- PC version (Windows/Mac/Linux)
- Mobile version (iOS/Android)
- Pixel-style download button

#### Installation Guide
- Step-by-step installation instructions
- Common questions and answers
- Pixel-style guide icons

### 7. Wallet Connection Function

#### Supported Wallets
- MetaMask
- WalletConnect
- Other mainstream wallets
- Pixel-style wallet icons

#### Connection Process
- Step description
- Security tips
- Pixel-style connection process diagram

#### Account Information
- Balance display
- Owned NFTs
- Transaction history
- Pixel-style account information panel

## Interactive Elements

### Button Design
- Pixel-style border
- Hover animation effect
- Click feedback effect

### Form Elements
- Pixel-style input box
- Checkbox and single-choice button
- Dropdown menu

### Loading Animation
- Pixel-style loading icon
- Progress bar design

### Popup Design
- Pixel-style border
- Close button
- Animation transition effect

## Responsive Design

### Desktop Version
- Full-function display
- Wide screen layout optimization

### Tablet Version
- Adapt to medium screen
- Touch-friendly interaction

### Mobile Version
- Simplified navigation (hamburger menu)
- Vertical layout optimization
- Touch-optimized button size

## Technical Implementation Suggestions

### Frontend Technology
- React/Next.js framework
- Tailwind CSS style
- Framer Motion animation
- Web3.js/ethers.js blockchain interaction

### Backend Technology
- Node.js server
- MongoDB database
- Blockchain API integration

### Blockchain Integration
- Smart contract interface
- NFT standard (ERC-721/ERC-1155)
- Multi-chain support

## Development Roadmap

### First Stage
- Home page and basic page structure
- Responsive design framework
- Basic wallet connection function

### Second Stage
- Complete page content
- NFT market basic function
- Community function

### Third Stage
- Advanced blockchain function
- Performance optimization
- Multi-language support

## Design Resource

### Pixel Art Resource
- Game character pixel map
- Environment elements
- UI components

### Font Selection
- Main title pixel font
- Body pixel font (ensure readability)

### Icon Library
- Navigation icons
- Function icons
- Social media icons

## User Experience Consideration

### New User Guidance
- Wallet connection tutorial
- Game entry guide
- Blockchain basic knowledge

### Loading Optimization
- Progressive loading
- Preload key resources
- Small game during loading

### Accessibility Design
- Color contrast consideration
- Keyboard navigation support
- Screen reader compatibility (while maintaining pixel style)

/// <reference types="next" />
/// <reference types="next/image-types/global" />

// NOTE: This file should not be edited
// see https://nextjs.org/docs/basic-features/typescript for more information.

"use client";

import Image from 'next/image';
import Link from 'next/link';

// NFT type definition
interface NFT {
  // Type definition remains unchanged
}

// Remaining code remains unchanged

## Packaging and Deployment Instructions

### Packaging the Website

To package the website into a ZIP file, run the following command:

```bash
npm run package
```

This will create a `dist` directory and generate a `website.zip` file containing all necessary website files.

### Deploying the Website

To prepare the website for deployment, run these commands:

```bash
npm run build   # First build the website
npm run deploy  # Then deploy the website
```

This will create a `deploy` directory containing all files needed for deployment, along with startup scripts:
- On Linux/Mac: Use `./start.sh`
- On Windows: Use `start.bat`

### Custom Deployment Directory

You can customize the deployment directory by setting the `DEPLOY_DIR` environment variable:

```bash
# On Linux/Mac
DEPLOY_DIR=/path/to/deploy npm run deploy

# On Windows
set DEPLOY_DIR=C:\path\to\deploy
npm run deploy
```

## Tech Stack

- **Frontend Framework**: Next.js 14
- **UI Library**: React 18
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Blockchain Integration**: ethers.js, wagmi, web3modal
- **Deployment**: Static Export + Node.js Server 