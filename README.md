# 🎮 Casino Game Platform

A full-featured casino gaming application built using **Node.js/Express** for the backend, **React.js/Redux** for the frontend, and **HTML Canvas** for rendering game graphics.

### 🎲 Available Games

- Roulette
- Blackjack
- Slot Machines
- Craps
- Poker (5 Card Draw & Texas Hold’em)
- Keno
- Race Betting

---

## 📋 Project Requirements

### 1. My opinions

### Strengths and weaknesses of UI/UX

**Strengths**

- **Strong, consistent casino look** — The green-and-gold palette and rabbit logo tie every screen together.
- **Clear, uncluttered layout** — Games are front and center, with simple “Play/Place” buttons and +/– bet controls.
- **Logical navigation** — Left menu for game categories, right panels for Info/Chat, keeps everything within reach.
- **Good use of space** — Ample margins and grouping make each screen feel open, not overwhelming.
- **Playful touches** — Bunny avatars and custom icons inject personality without clutter.

**Weaknesses**

- **Flat visual hierarchy** — Uniform borders and font weights make it hard to spot priority actions at a glance.
- **Sparse game graphics** — Empty slots reels and bare poker/blackjack layouts feel unfinished compared to industry standards.
- **No clear “home” or “lobby” button** — : users can get lost when switching games
- **Confusing back button icon** —  resembles “refresh” more than “go back”
- **Missing audio cues** —  no sound or visual confirmation when bets are placed or games start

### Crypto Payment Logic Assessment

- Integrated crypto payments using the NOWPayments API for multiple cryptocurrencies.
- The backend securely creates invoices, checks minimum payment amounts, and verifies payment status.
- All sensitive keys are stored in environment variables and never exposed to the client.
- Robust error handling provides clear user feedback.
- Payment flows are asynchronous and standardized for smooth frontend integration.

**Suggested Improvements**
- Add real-time payment status updates on the frontend.
- Support more cryptocurrencies and display their minimum payment amounts to users.
- Add transaction history for users to track their crypto payments.
- Enhance security by rotating API keys regularly and monitoring for suspicious activity.

### 2. Wallet Integration

- Integrated MetaMask wallet using **ethers.js** for secure and reliable wallet connectivity.
- Users are required to connect their MetaMask wallet before they can sign in—wallet connection is a **precondition** for authentication.
- The sign-in flow is preserved, but authentication is only possible after a successful wallet connection.
- All wallet-related prompts and messages are dynamically adjusted based on the selected language, ensuring a localized user experience.
