Generated list with Claude.ai

# GitHub Issues for lavender-daydream.com

Copy and paste these into GitHub Issues (one at a time). I've organized them by priority and added labels, descriptions, and task lists.

---

## HIGH PRIORITY ISSUES

### Issue #1: Integrate and maintain accessibility throughout website
**Labels:** `accessibility`, `high priority`, `enhancement`

**Description:**
Ensure the entire website follows accessibility best practices (WCAG 2.1 standards) as we continue development.

**Tasks:**
- [ ] Add ARIA labels to navigation elements
- [ ] Ensure all images have descriptive alt text
- [ ] Test keyboard navigation on all pages
- [ ] Check color contrast ratios (aim for WCAG AA minimum)
- [ ] Add skip-to-content links
- [ ] Test with screen readers
- [ ] Add semantic HTML5 elements where appropriate

**Resources:**
- [WebAIM Accessibility Checklist](https://webaim.org/standards/wcag/checklist)

---

### Issue #2: Improve splash page design and responsiveness
**Labels:** `design`, `high priority`, `mobile`

**Description:**
The splash page needs improvements to readability and mobile responsiveness.

**Tasks:**
- [ ] Make disclaimer text more readable
- [ ] Center the "Enter" button properly
- [ ] Position Panda icon:
  - Across from disclaimer on desktop
  - Above disclaimer on mobile
- [ ] Add content warning icons alongside Panda
- [ ] Test on various screen sizes

---

### Issue #3: Add "Currently/Current Hobbies" section to home page
**Labels:** `enhancement`, `high priority`, `content`

**Description:**
Add a section on the home page showing current hobbies/interests. Ideally, find a way to update this without editing HTML directly each time.

**Possible solutions:**
- Use a simple JSON file that gets loaded
- Create a small admin panel
- Use a static site generator
- Keep it simple with easy-to-find HTML section

---

### Issue #4: Complete About page (like Carrd)
**Labels:** `content`, `high priority`, `design`

**Description:**
Finish the About page with content similar to the Carrd version.

**Tasks:**
- [ ] Improve CSS styling
- [ ] Fill out Info/Quick Facts section
- [ ] Fill out Links section
- [ ] Write Introduction
- [ ] Write Bio
- [ ] Add Favorites section
- [ ] Add Interests section
- [ ] Create Quizzes section
  - [ ] Add "What Eva Character are you?" result (Shinji)

---

### Issue #5: Add and host Shantell Sans font
**Labels:** `design`, `high priority`, `fonts`

**Description:**
Self-host the Shantell Sans font instead of relying on external services.

**Tasks:**
- [ ] Download Shantell Sans font files
- [ ] Create `/Fonts` directory if needed
- [ ] Add font files to project
- [ ] Update CSS with `@font-face` declarations
- [ ] Test font loading across browsers
- [ ] Add font fallbacks

---

### Issue #6: Add update log section to home page
**Labels:** `enhancement`, `high priority`, `content`

**Description:**
Create a section on the home page showing recent updates and changes to the website.

**Possible format:**
- Reverse chronological list
- Last 5-10 updates visible
- Link to full changelog if needed

---

### Issue #7: Implement light and dark mode themes
**Labels:** `enhancement`, `high priority`, `design`, `accessibility`

**Description:**
Add theme switching capability starting with basic light and dark modes.

**Phase 1 (Priority):**
- [ ] Plain light mode
- [ ] Plain dark mode
- [ ] Theme toggle button
- [ ] Save user preference (localStorage)

**Phase 2 (Future):**
- [ ] Lined paper light mode
- [ ] Lined paper dark mode
- [ ] Clouds for light mode
- [ ] Night sky for dark mode
- [ ] Galaxy sky dark mode

---

## MEDIUM PRIORITY ISSUES

### Issue #8: Create custom buttons and blinkies
**Labels:** `design`, `enhancement`, `graphics`

**Description:**
Design custom buttons for the website and hoard page.

**Tasks:**
- [ ] Button for Button/Blinkie/Stamp hoard
- [ ] "Mother Mother Now!" button
- [ ] Add to appropriate pages

---

### Issue #9: Create and add favicons for all pages
**Labels:** `design`, `enhancement`

**Description:**
Design unique favicons (tab icons) for different sections of the website.

**Tasks:**
- [ ] Design main site favicon
- [ ] Design section-specific favicons (optional)
- [ ] Add favicon links to all HTML pages
- [ ] Test favicon display across browsers

---

### Issue #10: Create Characters hub page
**Labels:** `content`, `enhancement`, `large project`

**Description:**
Create a central hub page for all original and fanon characters, similar to ToyHouse organization.

**Structure:**
- Main Characters hub
  - Fanon Characters
  - Original Characters

**Tasks:**
- [ ] Create Characters hub/index page
- [ ] Design character card/profile layout
- [ ] Link from main navigation

**Related:** See separate issues for specific character pages

---

### Issue #11: Add Fanon Characters - JoJo AUs
**Labels:** `content`, `characters`, `mature content`

**Description:**
Create pages for JoJo's Bizarre Adventure AU characters. All pages need mature content warnings.

**Characters to add:**
- [ ] Frank Kekyoin
- [ ] Tenmei 'Taeko' Kakyoin
- [ ] Jotaro Joestar
- [ ] Reverse/Evil-Taro (name TBD)

**Requirements:**
- Each character needs profile page
- Mature content warning on all pages
- Art/images for each character
- Character bios and information

---

### Issue #12: Add Fanon Characters - Pokémon
**Labels:** `content`, `characters`, `PG`

**Description:**
Create pages for Pokémon original characters (PG rating).

**Characters to add:**
- [ ] Feenee (Delphox)
- [ ] Rocky (Midnight Lycanroc)
- [ ] Alimii (Altaria)
- [ ] Magnolia 'Maggie' (Sylveon)

---

### Issue #13: Add Fanon Characters - World of Warcraft
**Labels:** `content`, `characters`, `mature content`

**Description:**
Create page for WoW character (Teen or Mature rating).

**Character:**
- [ ] Victoria 'Roarlia' Harvest

---

### Issue #14: Add Original Characters pages
**Labels:** `content`, `characters`, `large project`

**Description:**
Create pages for original character stories/universes.

**Stories to add:**
- [ ] Imagination Blast (Teen)
- [ ] What's Righteous (PG or Teen)
- [ ] Felix and the Missing Leaves (G or PG)
- [ ] Symbolism Anthros/Sonas (Mature content warning)
  - [ ] Rich Pig (name TBD)
  - [ ] Innocent Lamb (name TBD - maybe Mollie?)
  - [ ] Black Cat Kawaii Punk (name TBD - maybe Marilynn?)

---

### Issue #15: Create Art page
**Labels:** `content`, `enhancement`, `gallery`

**Description:**
Create a dedicated art page/gallery showcasing artwork. Should integrate with character pages.

**Tasks:**
- [ ] Decide on gallery layout/style
- [ ] Organize art by category
- [ ] Add image optimization
- [ ] Add alt text to all artwork
- [ ] Link related character pages

---

### Issue #16: Create Recommendations/Resources page
**Labels:** `content`, `enhancement`

**Description:**
Create a page recommending apps, software, guides, and resources.

**Items to include:**
- [ ] Neocities
- [ ] VS Code
- [ ] PrivacyGuides.org
- [ ] Innuendo Studios: The Alt Right Playbook (YouTube playlist)
- [ ] Bitwarden
- [ ] Obsidian
- [ ] Firefox
- [ ] Ublock Origin
- [ ] Arab.org Click to Help Palestine

---

### Issue #17: Join and add webrings
**Labels:** `community`, `enhancement`, `links`

**Description:**
Research, join, and add webring badges to the website.

**Webrings to join:**
- [ ] JoJo's Bizarre Adventure Webring
- [ ] Oingo Boingo Web Ring
- [ ] Mother Mother Web ring
- [ ] Anti-Racism Webring
- [ ] Biseuxalism web ring (research status)
- [ ] Pokemon TCG Card Claim Clique
- [ ] Wii Ring
- [ ] Neo Creatives
- [ ] No AI Webring
- [ ] Catfolk Webring
- [ ] Ladies of the Link
- [ ] DS Ring
- [ ] Free Palestine Webring

---

### Issue #18: Join and add fanlistings
**Labels:** `community`, `enhancement`, `links`

**Description:**
Join relevant fanlistings and add badges to website.

**Fanlistings to join:**
- [ ] 3DS Fanlisting
- [ ] Braixen Fanlisting
- [ ] Altaria Fanlisting
- [ ] Midnight Lycanroc Fanlisting
- [ ] Pokemon X&Y Fanlisting
- [ ] Pokemon ORAS Fanlisting
- [ ] Pokemon Sun and Moon Fanlisting
- [ ] Sylveon Fanlisting
- [ ] Neko Atsume Fanlisting
- [ ] Jojo Fanlisting
- [ ] Jotaro Kujo Fanlisting
- [ ] Noriaki Kakyoin Fanlisting
- [ ] Foo Fighters (JJBA) Fanlisting
- [ ] Neon Genesis Evangelion Fanlisting

---

### Issue #19: Fill out Button/Stamp/Blinkie Hoard page
**Labels:** `content`, `hoard`

**Description:**
Complete the hoard page with organized collection of buttons, stamps, and blinkies.

**Tasks:**
- [ ] Organize by category
- [ ] Add descriptions/credits where appropriate
- [ ] Ensure images are optimized
- [ ] Add own custom buttons (see Issue #8)

---

### Issue #20: Add "Who is...?" page for people mentioned on site
**Labels:** `content`, `enhancement`, `privacy`

**Description:**
Create a page introducing people (IRL & online friends, family) mentioned throughout the website.

**Important rules:**
- **GET PERMISSION FIRST** before adding anyone
- Keep people anonymous if no permission
- Let people write their own profiles if desired
- Consider adding fictional characters too

**People to potentially add:**
- [ ] Bob (get permission)
- [ ] Dad/Darren (get permission)

---

### Issue #21: Update existing shrine pages
**Labels:** `content`, `shrines`, `update`

**Description:**
Complete and improve existing shrine pages.

**Shrines to update:**
- [ ] My 3DS (Teen rating)
- [ ] Minecraft Survival Adventures/Legends (PG or Teen)
- [ ] Jojo's Bizarre Adventure (Mature rating)
  - [ ] Jojo Memes subsection
- [ ] Neko Atsume (G rated)
  - [ ] Pasty Neko Atsume subsection

---

### Issue #22: Create new shrine pages
**Labels:** `content`, `shrines`, `enhancement`

**Description:**
Create new shrine pages for important subjects.

**New shrines to create:**
- [ ] Maizie (memorial for cat at Grandma's)
- [ ] Daphne (get permission first)

---

## LOW PRIORITY / FUTURE IDEAS

### Issue #23: Add current status section to home page
**Labels:** `enhancement`, `content`, `low priority`

**Description:**
Add a section showing current status/mood/activity (similar to status.cafe or MSN-style status).

**Considerations:**
- How to update easily
- Design/styling
- Privacy considerations

---

### Issue #24: Explore inspiration from 32bit.cafe and Neocities
**Labels:** `research`, `inspiration`, `low priority`

**Description:**
Browse through 32bit.cafe's website ideas and Neocities sites for inspiration and new features.

**Resources:**
- [32bit.cafe Website Ideas](https://32bit.cafe/websiteideas/)
- [Neocities Browse](https://neocities.org/browse)

---

## COMPLETED TASKS ✅

### ~~Issue #25: Make GitHub repo public~~
**Status:** COMPLETED! ✅

The repository is now public at: https://github.com/Lavender-Daydream/Website-lavender-daydream.com

---

## HOW TO USE THESE ISSUES

1. **Copy each issue one at a time**
2. **Go to your GitHub repo** → Issues tab → New Issue
3. **Paste the title** (the "Issue #X:" part)
4. **Paste the description and tasks** in the body
5. **Add the labels** mentioned (you may need to create some custom labels first)
6. **Submit the issue**

## SUGGESTED LABELS TO CREATE

Go to Issues → Labels → New Label and create these:

- `accessibility` (color: #0052CC) - Accessibility improvements
- `high priority` (color: #D93F0B) - High priority tasks
- `design` (color: #FBCA04) - Design and styling
- `content` (color: #0E8A16) - Content creation
- `enhancement` (color: #84B6EB) - New features
- `mobile` (color: #D4C5F9) - Mobile responsiveness
- `fonts` (color: #C5DEF5) - Font-related tasks
- `graphics` (color: #F9D0C4) - Graphics and images
- `characters` (color: #BFD4F2) - Character pages
- `shrines` (color: #FEF2C0) - Shrine pages
- `hoard` (color: #C2E0C6) - Hoard page
- `community` (color: #BFDADC) - Community/webrings/fanlistings
- `links` (color: #E99695) - External links
- `mature content` (color: #B60205) - Mature content warning needed
- `PG` (color: #D4C5F9) - PG rated content
- `large project` (color: #5319E7) - Large/complex projects
- `privacy` (color: #1D76DB) - Privacy considerations
- `research` (color: #EDEDED) - Research needed
- `inspiration` (color: #FEF2C0) - Inspiration/ideas
- `low priority` (color: #E4E669) - Low priority tasks
- `good first issue` (color: #7057FF) - Good for beginners/contributors

---

## TIPS

- **Start with high priority issues** (Issues #1-7)
- **Break down large projects** (like Issue #10) into smaller sub-issues if needed
- **Close issues as you complete them** - it feels great!
- **Reference issues in commits** with "closes #X" or "fixes #X"
- **Use milestones** to group related issues (e.g., "Accessibility Overhaul", "Character Pages Complete")
- **Add screenshots** to design-related issues when you have them
- **Update issues** as you make progress or learn new information

Good luck with your website! 🌟
