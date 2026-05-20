# Restaurant Booking Agent (Hermes Agent Skill)

An AI-powered front-of-house assistant that handles reservations, menu questions, dietary accommodations, and customer service — deployed on WhatsApp, Telegram, or any messaging platform via Hermes Agent.

## What It Does

- Takes reservation requests (date, time, party size, name, phone)
- Answers menu and dietary questions (halal, vegan, gluten-free)
- Handles hours, location, delivery info
- Natural upselling (sharing platters for groups, weekend specials)
- Escalates complaints to human manager
- Works 24/7 on WhatsApp, Telegram, SMS
## Live Demo
[Watch the agent in action on Telegram]https://streamable.com/1la8xd
## Demo Conversation

> **Customer:** Hi, I'd like to book a table for 4 this Saturday at 7pm
>
> **Agent:** To get your reservation sorted, I just need a couple more details:
> 1. What name should the booking be under?
> 2. And a phone number we can reach you on?
>
> Also, Saturday evenings are a great time to visit — we have some lovely weekend specials on. And for a group of 4, our sharing platters are always a big hit if you're interested!
>
> Looking forward to welcoming you.

## Setup

```bash
# Install Hermes Agent
curl -fsSL https://raw.githubusercontent.com/NousResearch/hermes-agent/main/scripts/install.sh | bash

# Copy skill
cp -r . ~/.hermes/skills/restaurant-agent/

# Start chatting
hermes chat
```

## Customization

Edit the `Restaurant Details` section in SKILL.md to match your client's restaurant — name, hours, menu, location, dietary options. Deploy in under 30 minutes.

## Built With

- [Hermes Agent](https://github.com/NousResearch/hermes-agent) by Nous Research
- Claude Sonnet 4.6 (Anthropic)
- MIT License

