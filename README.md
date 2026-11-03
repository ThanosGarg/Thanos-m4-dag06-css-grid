# Day 6 · CSS Grid

*Module 4, UI/UX & Frontend Development, Lexicon IT-Proffs*

## What you will do today

You will build the menu grid and the About Us section layout using CSS Grid.

## Background

Grid arranges elements in **two dimensions**: rows and columns at the same time. The rule of thumb to remember: **Grid for the overall layout, Flexbox inside.** Today you will build a responsive grid without a single media query.

## Workflow (the same as always)

1. **Fork** today's repository on GitHub (*Fork → Create fork*).
2. **Clone your fork:** *Code → HTTPS → copy the URL*. In the terminal (Ctrl+ö in VS Code): `git clone <url>`. Open the new folder in VS Code and start *Live Server*.
3. **Complete the assignment.** Save and check in the browser after each step. Make a commit after each completed step: `git add .` and `git commit -m "Describe what you did"`.
4. **Push** when you are done: `git push`.
5. **Submit through Microsoft Forms.**

If you get stuck, write down exactly where you got stuck and what you have tried, and bring it up first in the next guided session.

## The assignment, step by step

### Step 1. Turn the menu into a grid

Make `.meny-lista` (the div containing the three cards) a grid container. Start with `grid-template-columns: 1fr 1fr 1fr` and observe the three columns. Add `gap: 20px`. Remove `margin-bottom` from the cards inside the grid; `gap` handles the spacing.

### Step 2. Make it flexible

Replace the column definition with `repeat(auto-fit, minmax(240px, 1fr))`. Resize the browser window and watch the number of columns adjust automatically.

### Step 3. About Us in two columns

Make `#om-oss` a grid. Place the paragraphs in one column and the image in the other. The heading should span both columns: `grid-column: 1 / -1`.

### Step 4. Use the grid overlay

In DevTools, click the `grid` icon next to the element. The rows and columns will be outlined. Take a look at the line numbers.

### Step 5. Explicit placement

Place the image in column 2 using `grid-column: 2` and `grid-row`. Experiment with swapping the positions of the text and image.

### Step 6. Explain your choice

For each layout, add a comment stating "Grid" or "Flexbox" and explaining why.

## Checklist: how to know you are done

- [ ] The menu is a grid that changes its number of columns without media queries.
- [ ] The About Us heading spans both columns.
- [ ] About Us has a two-column layout.
- [ ] You have used `gap`.
- [ ] You have explained your choice between Grid and Flexbox in comments.
- [ ] You have pushed to your fork and submitted the link.

## Tips if you get stuck

- `fr` is a fraction of the available space: `1fr 2fr` makes the second column twice as wide.
- Is a child element in the wrong place? Check whether it has explicit `grid-column` values.
- Sketch the columns on paper if you lose track.

## Submission

**Deadline: tomorrow at 09:00.** Submit everything through Microsoft Forms. No oral presentation is required.

Fill in the following in the form:

1. A link to your fork of this repository.
2. Reflection: Explain the rule of thumb "Grid for the overall layout, Flexbox inside" using your own example from the café's page.

## Want to do more? (optional)

- Rebuild the entire page using `grid-template-areas` (header, main, footer).
- Create an image gallery section in About Us with a nested grid.
