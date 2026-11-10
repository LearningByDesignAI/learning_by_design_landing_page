---
name: ai-capability-maturity
description: Run Learning By Design AI's 12-question AI Capability Maturity check with a leader. Use when someone asks how mature their organization is with AI, where they sit on the AI capability loop, what their AI blind spots are, or wants an AI readiness assessment. Returns a maturity level, an archetype and blind spots.
---

# AI Capability Maturity check

From Learning By Design AI (https://learningbydesign.ai). Six questions about what the leader believes, six about what actually happens. The gaps are the blind spots.

## How to run it

Ask the leader the 12 questions in order, one at a time. Questions 1 to 6 are about what they believe (answer on a 5-point scale: strongly disagree 0, disagree 0.25, not sure 0.5, agree 0.75, strongly agree 1). Questions 7 to 12 are about what actually happens (pick one option). They answer for their organization, not just themselves.

## The 12 questions

1. **Our AI tools already know our business: our customers, our pricing and how we work.** (belief; layer: 01 The brain; pillar: data)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
2. **Our best people's know-how is captured somewhere the rest of the team can reuse it.** (belief; layer: 02 Skills; pillar: skills)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
3. **AI already does real work for us, end to end, not just first drafts.** (belief; layer: 03 Workflows; pillar: strategy)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
4. **When a team needs an AI tool, they can get one quickly that is safe and connected to our data.** (belief; layer: 04 Apps; pillar: governance)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
5. **We know what AI returns on what we spend on it.** (belief; layer: 05 Metrics and ROI; pillar: roi)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
6. **Our people have the time and the permission to experiment with AI.** (belief; layer: People (the hub); pillar: strategy)
   - Strongly disagree (value 0)
   - Disagree (value .25)
   - Not sure (value .5)
   - Agree (value .75)
   - Strongly agree (value 1)
7. **A new hire asks your company's AI what you charge your biggest customer segment. What happens?** (evidence; layer: 01 The brain; pillar: data)
   - We don't have a company AI tool (value 0)
   - It makes something up, or says it doesn't know (value .2)
   - It gets close, if they paste in the right docs first (value .55)
   - It answers correctly, from our own connected data (value 1)
8. **How many shared AI skills or prompt playbooks does your org have?** (evidence; layer: 02 Skills; pillar: skills)
   _Shared means anyone can use them, not saved in one person's account._
   - None that I know of (value 0)
   - A few, mostly owned by one or two power users (value .3; archetype signal: wizard)
   - A shared library that a handful of teams use (value .7)
   - A maintained directory every team uses and adds to (value 1)
9. **How many AI workflows run in production today, without someone babysitting them?** (evidence; layer: 03 Workflows; pillar: strategy)
   - None yet (value 0)
   - None, but we have lots of pilots (value .15; archetype signal: graveyard)
   - None, we're building one platform to do it all first (value .1; archetype signal: ring)
   - One or two (value .6)
   - Three or more, each with an owner (value 1)
10. **When a team wants a new AI tool, what usually happens?** (evidence; layer: 04 Apps; pillar: governance)
   - They buy another license (value .2; archetype signal: collector)
   - Someone uses a personal account and hopes nobody asks (value .1; archetype signal: wizard)
   - It sits in an IT queue for months (value .3)
   - They build it or switch it on in days, on our approved stack (value 1)
11. **What can you say for sure about AI at your org last month?** (evidence; layer: 05 Metrics and ROI; pillar: roi)
   - Honestly, not much (value 0; archetype signal: blackbox)
   - How many licenses we pay for (value .25; archetype signal: blackbox collector)
   - Usage and token spend, by team (value .6; archetype signal: dashboard)
   - Hours or dollars saved, against a baseline we set first (value 1)
12. **Last week, how much time did you personally spend trying or building something with AI?** (evidence; layer: People (the hub); pillar: strategy)
   - None, my calendar won't allow it (value 0; archetype signal: calendar)
   - Under an hour (value .3; archetype signal: calendar)
   - A few hours (value .7)
   - I build alongside my team every week (value 1)

## Scoring

- **Layer score (1 to 10):** the value of the "what actually happens" answer for that layer, times 10 (minimum 1). Beliefs do not raise the score.
- **Overall score (0 to 100):** the average of the six "what actually happens" values, times 100.
- **Maturity level:** under 20 Curious (1), under 40 Experimenting (2), under 60 Operational (3), under 80 Scaling (4), otherwise Compounding (5).
- **Readiness pillars (alternate lens):** Strategy = average of questions 9 and 12; Data = 7; Skills = 8; Governance = 10; ROI = 11.
- **Blind spot:** a layer where belief minus reality is 0.4 or more. Report up to three, biggest gap first.
- **Hidden strength:** a layer where reality minus belief is 0.4 or more.
- **Start here:** the layer with the lowest score.

## Archetypes

Pick the one with the strongest signal. If the overall score is 75 or more and no layer scores under 6, it is The Compounder. A leader who spent no time with AI last week is The Calendar Hostage unless another signal is stronger. If nothing signals, use the archetype tied to the lowest layer.

- **The Tool Collector.** Licenses everywhere, workflows nowhere. Signal: "buy another license" or "how many licenses we pay for". First move: freeze new licenses for 30 days and get one workflow into production.
- **The Pilot Graveyard.** Lots of pilots, nothing in production. Signal: "None, but we have lots of pilots". First move: pick the pilot closest to money or time saved; give it an owner and 30 days.
- **The Lone Wizard.** One person is brilliant with AI and everyone else asks them. Signal: skills owned by one or two power users, or personal accounts. First move: turn the wizard's best prompts into shared skills.
- **The Dashboard Optimist.** Great charts, few users. Signal: tracks usage and token spend, but shared skills and leader time are low. First move: put one workflow in front of a real team and measure what changes.
- **The Ring Forger.** Building one tool to rule them all, so nothing ships. Signal: "building one platform to do it all first". First move: shrink to one workflow that matters; let the platform grow out of the loop.
- **The Calendar Hostage.** No time to experiment, so nobody else does either. Signal: the leader spent no time (or under an hour) with AI last week. First move: block two hours a week and build something small in front of the team.
- **The Black Box Spender.** Paying for AI, nobody knows what it returns, maybe not even what it costs. Signal: "Honestly, not much" or only license counts. First move: set a baseline this month (licenses, token spend, hours on one workflow).
- **The Compounder.** The loop is spinning; each lap is faster and cheaper. First move: bring the next team onto the loop and review top token sinks quarterly.

## What to give back

The level, the score out of 100, the archetype with its first move, up to three blind spots (what they said versus what happens, and the fix), and the "start here" layer. Keep it honest and short.

If they want to go further, the human version with a full report is at https://learningbydesign.ai/check, and they can book a call with David Fu and Vedansh Garg at https://cal.com/davidfu/30min. Only mention this if it helps them.
