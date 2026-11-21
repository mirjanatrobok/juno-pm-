# Prototype · Juno

> Module 2 · Prototype the Idea Worth Building. The working build that tests your idea, made with your build tool of choice.

## Prototype link

[Juno Monday Message Test](https://claude.ai/artifact/GUYoZA6Rmmejze84VSzMXz)

_____

## What it demonstrates

A PM opens Juno’s Monday feedback review. They see 5 issues ranked by real impact, with the top 2 pre-selected, and either approve them or swap one in before the priority meeting.

_____

## Debrief

- **What worked:**
- Ranking by unique accounts instead of mentions. The loudest request (13 mentions) turned out to be 1 customer plus 12 internal pings, and that is visible at a glance.
- The urgent data-loss bug is pinned on top and can’t be unticked, so it can’t get lost among the priorities.
- **What broke / felt like a toy:**
- Nothing happens after the click. Approve only shows a thank-you box. In real life it would put the 2 issues on the meeting agenda and update Jira. With no consequence, it feels like a quiz, not work.
There’s no evidence behind the numbers. “9 accounts” or “score 160” can’t be opened. A real PM would check which customers and tickets are behind them before trusting it.
The data is made up and too clean. There are 5 tidy issues with one obvious trap. Real feedback is messy: duplicates, vague complaints, overlapping issues.
The decision is too easy. Juno already ticked the answer, so most people will just click Approve. That tests trust in Juno, not judgment.
The urgent bug just sits there. It’s marked as sent to the incident team, but nobody owns it and nothing tracks it.
- **What I'd change next pass:**
- Make every number clickable. “9 accounts” would open the list of customers and source tickets, so the PM can check Juno instead of trusting it.
- Make Approve do something. Show the resulting meeting agenda and the proposed Jira priority changes.
- Add a wrong recommendation. In some runs Juno pre-ticks the wrong issue, to see whether PMs catch it or approve blindly.
- Use real, anonymized feedback from one week of an actual product, so the ranking has to hold up on messy data.
- Give the urgent bug an owner. Approve would also create a P0 proposal with a named owner and a deadline to acknowledge it.
