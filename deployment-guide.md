# C.H.E.A.T. Code™ Diagnostic: Deployment Guide

## Files Ready to Deploy

- `index.html` — Standalone diagnostic (push this to GitHub)
- `og-image.png` — 1200x630 social sharing image
- `cheat-code-diagnostic.jsx` — React source (keep as reference)

---

## Step 1: GitHub Repo + Pages

Run these commands in your terminal (replace quietrebellion):

```bash
mkdir cheat-code-diagnostic
cd cheat-code-diagnostic
git init
# Copy index.html and og-image.png into this folder, then:
git add .
git commit -m "C.H.E.A.T. Code Diagnostic v1"
git branch -M main
git remote add origin git@github.com:quietrebellion/cheat-code-diagnostic.git
git push -u origin main
```

Then in GitHub:
1. Go to your repo → Settings → Pages
2. Source: Deploy from a branch
3. Branch: main, folder: / (root)
4. Save
5. Wait 1-2 minutes, your site is live at: `quietrebellion.github.io/cheat-code-diagnostic`

---

## Step 2: Update index.html Before Going Live

Open index.html and make these changes:

**Line 1 of the script block:**
Replace `YOUR_DRIP_CAMPAIGN_FORM_ID` with your ConvertKit form ID.
Find it in ConvertKit: Forms → your drip campaign form → Settings → the number in the URL.

**OG meta tags in the head (lines 11-12):**
Uncomment and update:
```html
<meta property="og:image" content="https://quietrebellion.github.io/cheat-code-diagnostic/og-image.png">
<meta property="og:url" content="https://quietrebellion.github.io/cheat-code-diagnostic">
```

**Calendly link:**
Confirm `rebellioncollective.com/application-form` is still active. If it changed, search and replace in the file (appears twice: once in the diagnostic, once in the PDF).

---

## Step 3: Squarespace Integration

**Option A: Iframe embed**
Create a new page at rebellioncollective.com/diagnostic. Add a Code Block with:
```html
<div style="width:100%;min-height:100vh;margin:-40px 0">
<iframe src="https://quietrebellion.github.io/cheat-code-diagnostic" style="width:100%;height:100vh;border:none" title="C.H.E.A.T. Code Diagnostic"></iframe>
</div>
```

**Option B: Redirect**
In Squarespace: Settings → URL Mappings, add:
```
/cheatcode -> https://quietrebellion.github.io/cheat-code-diagnostic 302
```

---

## Step 4: ConvertKit Drip Campaign

Create a new form in ConvertKit specifically for the diagnostic (separate from Dispatches).
Create an automation sequence triggered by that form subscription.
Schedule: one email per week, five weeks total.

---

## 5-Part Drip Campaign: Email Copy

### Email 1: Curiosity (Week 1)

**Subject:** Your diagnostic results start here

**Body:**

You took the C.H.E.A.T. Code™ Diagnostic. That means you're already doing the first thing most people skip: looking.

Curiosity is the first habit for a reason. Before you can change your equation, you have to see what's running it.

This week, try one thing.

Pick whichever version fits where you are right now:

If your attention feels scattered: track it for 48 hours. Sixty-minute blocks. What are you doing? Did you choose to be there? Write it down. The data will be uncomfortable and clarifying in equal measure.

If your head feels full: get every open loop onto paper. Every half-finished decision, lingering obligation, unresolved question. All of it. Your working memory is full. Empty it somewhere you can see it.

If you feel pulled between past and future: three times today, pause for one breath and ask yourself where your attention actually is right now. You don't need to fix anything. Just see it clearly.

Curiosity isn't about solving anything yet. It's about naming what's true.

Next week: Courage.

Nicholas Whitaker
Rebellion Collective

---

### Email 2: Courage (Week 2)

**Subject:** What you found might be uncomfortable

**Body:**

Last week was about looking. This week is about what happens when you don't like what you see.

Curiosity surfaces the pattern. Courage is what moves you toward it instead of away. Most people skip this step by staying busy, renaming avoidance as responsibility, or waiting for the "right time" that never arrives.

This week, try one thing.

If your work feels misaligned: ask yourself what you're calling responsibility right now that might actually be fear. Sit with the answer. Then choose one thing to renegotiate this week. One.

If you're carrying emotional weight: name the conversation you've been avoiding. The one that costs you energy every day you delay it. Put it on the calendar this week and walk in with data, no drama.

If neither of those fit: ask yourself where you're holding on out of fear. The cost of staying is real even when you can't see it on a spreadsheet.

Courage doesn't require certainty. It requires honesty.

Next week: Compassion.

Nicholas Whitaker
Rebellion Collective

---

### Email 3: Compassion (Week 3)

**Subject:** The second arrow

**Body:**

In Buddhist teaching, pain is the first arrow. The story you tell yourself about the pain is the second arrow. Most of us are walking around full of second arrows.

Compassion is the habit that stops the second shot. Without it, curiosity becomes self-criticism and courage becomes grinding. You find the hard thing and then beat yourself up for it. That's the pattern compassion interrupts.

This week, try one thing.

If you're running on fumes: your body is keeping score. Choose one thing this week: sleep, movement, or nourishment. Treat it as sacred. The same way you'd protect a meeting with your most important client. You are that client.

If the inner critic is loud: next time you catch it, try the RAIN practice. Recognize what's happening. Allow it to be there. Investigate it with kindness. Nurture yourself through it. It takes ninety seconds.

If you're stuck in your head: drop into your body. Where do you feel it? How big is it? Bring five percent of your attention to naming it and ninety-five percent to the direct sensation. Stay there for three breaths.

Compassion is the floor that holds when everything else is shaking.

Next week: Connection.

Nicholas Whitaker
Rebellion Collective

---

### Email 4: Connection (Week 4)

**Subject:** When was the last time someone really saw you?

**Body:**

Connection is the habit most high-performers deprioritize first. Time with other humans feels inefficient. Unstructured presence feels unproductive. So we optimize it away and wonder why the work feels hollow.

Connection restores meaning. Time stops feeling consumed and starts feeling alive. But it requires something most of us have been trained out of: visibility.

This week, try one thing.

If your calendar owns you: find one block this week spent on obligations that drain you. Replace it with unstructured time with someone who fills you up. Let the conversation go wherever it goes.

If your relationships feel transactional: think of three people you interact with regularly. For each one, ask: what do I bring to their equation? Do I add energy or drain it? Do I give them my attention or just my time?

If you're isolated: reach out to one person today. Someone you trust. Tell them something true about where you are right now. Connection starts with visibility.

Next week: Commitment. The one that holds everything together.

Nicholas Whitaker
Rebellion Collective

---

### Email 5: Commitment (Week 5)

**Subject:** The smallest honest move

**Body:**

You've spent four weeks looking at your pattern. Curiosity to see it. Courage to face it. Compassion to hold yourself through it. Connection to let someone else in.

Commitment is what makes it stick.

Not commitment as discipline or willpower. Commitment as practice. Protecting your capacity. Staying curious, courageous, compassionate, and connected. Every day. Even imperfectly. Especially so.

This week, try one thing.

If your boundaries don't hold: block one hour this week that belongs to you. Label it. Defend it. When someone tries to take it, practice the full sentence: no. That boundary is the seed of every other boundary.

If you're still carrying obligations that no longer serve you: name one recurring commitment you already know needs to go. Drop it, delegate it, or renegotiate it this week. Recovered time is the first resource you reinvest.

If you're not sure where to start: ask yourself what's the smallest honest move you could make before the end of this week. Say it out loud to someone you trust. That's what makes it real.

This is the end of the series, but not the end of the work. If you want to go deeper into your pattern, the Clarity Call is where that conversation happens. Forty-five minutes. We review your diagnostic, explore what's underneath the numbers, and talk about what comes next.

Book a Clarity Call: https://rebellioncollective.com/application-form?utm_source=cheat_drip&utm_medium=email&utm_campaign=habit5

Reclaim what's yours.

Nicholas Whitaker
Rebellion Collective
