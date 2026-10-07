# Skill-Swap-AI-Prototype

## Context:

Skill Swap is a mobile app I designed that matches adults through skills they can teach and want to learn. The goal was fewer, better matches and an easy first conversation. Full case study: https://taliyajlewis.com/skill-swap 

## Process

Prompt 1. [ Build a clickable HTML prototype of this flow: (Here I provided images of High Fidelity Concepts I created in Figma and Skill Swap design brief.)

Requirements: Include an empty state for no sessions and an error state if joining fails, use large touch targets, and keep it in one HTML file. After the prototype, briefly explain the main design decisions you made and anything you were unsure about. ]

Result: [Initial working prototype generated; 

Main Design Decisions: 

The swap is the headline. Every match card leads with a split tile: "Madison teaches you Cooking ⇄ You teach Madison Photography." A blue edge marks what you learn and a red edge marks what you teach. Avatars are initials, so photos support the profile rather than lead it. This is the one bold element. Everything around it follows plain Carbon: square corners, IBM Plex Sans, 8px spacing, and fields with a bottom border.

Fewer, better matches. The feed shows exactly three people, ranked by how mutual the swap is, and then ends with "You're all caught up." I left out the skill filter chips from your Home frame because they push toward browsing volume, which works against the curated feed.

Easy openers. Each card shows a conversation starter tied to the shared skill. "Say hi" puts it into the composer so the user can edit it before sending. An empty chat offers three starters. This targets your "first message without hesitation" metric while keeping the user in control.

The swap is explained at first use. The three-step explanation appears on the welcome screen and again as a sheet when someone first reaches Home after setup. It uses their own skills, like "like photography." An info button in the header reopens it from anywhere.

Navigation stays put. The header and the bottom nav stay fixed while the content scrolls. I used four labeled tabs: Home, Swaps, Messages, Profile. Your frames had three tabs, with Swaps tucked inside Messages, but sessions and conversations are different jobs. Badges show unread messages and incoming swap requests.

Accessibility. All touch targets are at least 48px tall. Your brand red (
#E43D4C) gets only 4.1:1 contrast with white text, so filled buttons use a darker shade (
#C92F3E), which passes AA. The bright brand colors still appear in the logo, accents and avatars. The prototype also has a dark theme that follows the system setting.]

Things I wasn't sure about: 

- Bottom nav in chat: I hid it inside a conversation to honor "low clutter in messaging," but that partly conflicts with "persistent navigation." It's worth testing.

- Matching. It's simulated with keyword overlap, so unusual skills entered during sign-up produce weaker "New skill" matches. The brief doesn't say whether the location step should ask for permission or just accept typed input, so I did both.

## What I rejected and changed: 
- Rejected: Prompt 2 [Switch to a light theme that matches my attached Figma screens: white background, the blue-to-red gradient only on the welcome screen, and the red and blue brand colors for actions. Keep the layout and content otherwise, and keep text contrast at least 4.5:1.]

Result: [updated the same prototype link. It now uses a light theme only, and the layout and content are unchanged.

What changed: 

One light theme. The dark-mode version is gone, so every screen has a white background with light gray tiles. This holds even when your device is set to dark mode.
Gradient only on welcome. The welcome hero is the only place with the blue-to-red gradient. The profile banner, which was also a gradient, is now solid brand blue.
Red and blue for actions. Primary actions are red: Get started, Say hi, Propose swap, Join circle, Send. Secondary actions like View profile, Message and Back changed from dark gray to brand blue. The selected Matches/Circles toggle is blue, like the "All skills" pill in your Figma. The active bottom-nav tab gets a blue top bar.

Where contrast meant small adjustments

I measured every text and background pair. All of them now meet 4.5:1, and the lowest is 4.57:1 for placeholder text.]

Hand Edits: 