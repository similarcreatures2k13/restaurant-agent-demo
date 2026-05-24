# Restaurant Booking Agent (Hermes Agent Skill)

An AI-powered front-of-house assistant that handles reservations, menu questions, dietary accommodations, and customer service — deployed on WhatsApp, Telegram, or any messaging platform via Hermes Agent.

## What It Does

- Takes reservation requests and books them on Google Calendar automatically
- Answers menu and dietary questions (halal, vegan, gluten-free)
- Handles hours, location, delivery info
- Natural upselling (sharing platters for groups, weekend specials)
- Escalates complaints to human manager
- Works 24/7 on WhatsApp, Telegram, SMS

## Demo Conversation

> **Customer:** Hi, I'd like to book a table for 4 this Saturday at 7pm
>
> **Agent:** To get your reservation sorted, I just need a couple more details:
> 1. What name should the booking be under?
> 2. And a phone number we can reach you on?
>
> Saturday evenings are a great time — we have lovely weekend specials on. And for a group of 4, our sharing platters are always a big hit!

## Google Calendar Integration

When a booking is confirmed, the agent creates a real calendar event automatically — no manual entry needed.

## Setup

1. Install [Hermes Agent](https://github.com/NousResearch/hermes-agent)
2. Copy `SKILL.md` to `~/.hermes/skills/restaurant-agent/`
3. Set up Google Calendar credentials (see `calendar_tool.py`)
4. Run `hermes chat` and start taking bookings

## Customization

Edit the Restaurant Details section in SKILL.md to match your client's restaurant — name, hours, menu, location, dietary options. Deploy in under 30 minutes.

## Built With

- [Hermes Agent](https://github.com/NousResearch/hermes-agent) by Nous Research
- Claude Sonnet 4 (Anthropic)
- Google Calendar API
- MIT License
