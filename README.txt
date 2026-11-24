SpecSmart: concept laptop store with an AI advisor (SC45WORKS portfolio)
=======================================================================

SpecSmart is a fictional neighbourhood laptop store in Austin, Texas. The
store, laptops, prices and stock are invented, and the page says so in the
top ribbon and footer. The name was checked against real stores in
November 2026.

SUGGESTED ADDRESS
  specsmart.sc45works.com. The page has a "noindex" tag so search engines
  don't list a fake store.

HOW THE ADVISOR WORKS
  1. The shopper picks a use (work, everyday, creative, gaming), a budget
     and optional extras (all-day battery, light, big screen).
  2. The page scores every laptop in stock on seven specs (CPU, RAM, GPU,
     storage, battery, weight, screen) against what that use needs, and
     shows the top three with a verdict per spec: WORTH IT, SKIP IT,
     NICE TO HAVE, FINE, or BELOW NEED.
     This part is plain code in index.html (look for STOCK and NEEDS), so
     it's instant, free and always works.
     Gaming asks four follow-ups (game type, graphics settings, resolution,
     screen size) and Creative asks two (what you create, project size), so
     the GPU, RAM, CPU, storage and screen targets scale with the answers.
     Esports checks for a 144Hz+ screen; 4K checks for a 4K panel; photo,
     design and video check for an OLED or color-accurate screen.
  3. The page re-themes per use: Work calm blue, Everyday warm yellow,
     Creative violet-pink, Gaming dark with neon green. A soft cursor glow
     in the mood's colour lights the nearby dots (desktop only; off for
     visitors who ask for reduced motion).
  4. If a big budget isn't needed, it says so and suggests cheaper laptops.
     If a budget is too small for the use, it warns and names the cheapest
     laptop that does the job properly. For 4K ultra in the newest AAA
     games, it also says even top laptop GPUs need upscaling like DLSS.
  5. "Ask the advisor" is the AI part: Claude answers follow-up questions
     using the shopper's answers, their three picks and the stock list.

DEPLOY
  Same as your other sites: Vercel (GitHub import or "npx vercel"), or
  Netlify via GitHub. Add ANTHROPIC_API_KEY as an environment variable and
  redeploy. Without a key, "Ask the advisor" falls back to built-in answers.

FOR A REAL STORE
  Replace the STOCK list with the store's live inventory (from its POS or a
  Google Sheet), and connect "Reserve for pickup" to its booking or CRM.
