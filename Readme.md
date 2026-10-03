<div align="center">

🧮 SC88

Une calculatrice, cinq humeurs. Rien de plus.

</div>

---

👋 Welcome

Every calculator app on my phone is either too much or too little.

Too much: the one that ships with the OS, which has a scientific mode, a graphing mode, a unit converter, a currency converter, a "Tip" screen I've never once used, and an ad for the Pro version that appears every third launch. Too little: the back of an envelope, which I keep losing.

SC88 is the one in the middle. It does addition, subtraction, multiplication, division, percent, and decimals. It has a clear button, a backspace, and an equals sign. That's the entire feature set. But it does those things with taste.

The design is the point. One calculator, five themes, each one drawn from a different aesthetic universe. Same math underneath, completely different object on the screen. A blue minimal calculator from 2015. A terracotta-and-grain retro one. A sepia thing that looks like it fell out of a hardback novel. A teal tarot card with double borders. And a pink pop-art one with thick black outlines and buttons that physically press down when you tap them.

Click SWITCH THEME and the whole app changes character. The display border, the fonts, the shadows, the corner radii, the colour of every key — they all shift together. It's the same calculator, in a different mood.

It's fast. It responds to your keyboard as well as your touch. And it lives in one HTML file with no dependencies except the Google Fonts it loads for the five themes.

---

<!--
## 📸 Look Inside

<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/sc88/raw/main/images/preview-1.png" alt="Theme 1 — Minimalist Blue" width="100%" />
  <br />
  <sub><b>① Minimalist Blue</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/sc88/raw/main/images/preview-2.png" alt="Theme 3 — Vintage Sepia" width="100%" />
  <br />
  <sub><b>② Vintage Sepia</b></sub>
</div>

<br />
<br />

<div align="center">
  <img src="https://github.com/mohamed005cheikh-rgb/sc88/raw/main/images/preview-3.png" alt="Theme 5 — Pink Pop-Art" width="100%" />
  <br />
  <sub><b>③ Pink Pop-Art</b></sub>
</div>
-->

---

✨ What you'll find

Five themes, one button apart.
The button in the header cycles through them all. Each theme is a completely different calculator, not a colour swap:

· Minimalist Blue — soft blue background, rounded white keys, orange operator buttons, sans-serif. The one you'd find on a well-designed Android phone in 2016.
· Terracotta & Grain — burnt orange and cream, Courier Prime monospace, a screen that glows green like an old terminal. Feels like typing on a mechanical typewriter that does math.
· Vintage Sepia — brown leather background, Playfair Display serif, ivory keys with hard black borders, a display that looks like a page torn from an antique ledger. Academic, quiet, patient.
· Tarot Teal — Cinzel serif, double-bordered display, muted greens and teals. Looks like something you'd draw a card from.
· Pink Pop-Art — hot pink background, Fredoka type, thick black outlines everywhere, chunky drop shadows, and keys that visibly depress when you tap them. Loud, happy, comic-book.

All five arithmetic operations, done well.
Addition, subtraction, multiplication, division, and percent. The percent key divides the current number by a hundred — plain and honest, no contextual guessing. Division by zero doesn't crash the app; it shows Error and waits for you to press AC.

A live expression line above the result.
As you type, the small line above the big number shows what you're building: 12 +  while you wait, then 12 + 8 = when you press equals. It's small, italic in some themes, and it stays out of the way. But it means you never wonder what operation is pending.

Smart number formatting.
Thousand separators (1,234,567) appear as you type. Long results shrink automatically — first to a smaller size, then smaller again — so nothing ever overflows the display. Results too large or too small for the number display switch to exponential notation (1.234567e+15) on their own.

Twelve digits, then it stops.
You can't type a thirteenth digit. Twelve is the working limit, chosen so the display stays readable on any screen size. It's enough for phone numbers, most prices, and almost anything you'd type into a calculator by hand.

Chained operations that behave.
Press 5 × 3 + 2 = and you get 17, not 10. Every time you press an operator, the pending one resolves first — the way a real calculator has always worked. If that feels obvious, good — many calculator apps get it wrong.

Keyboard support for everything.
Type numbers, . (or , — both work), the four operators, Enter or = to evaluate, Escape or C to clear, Backspace to delete, % for percent. Every key press flashes the corresponding on-screen button so you can see what the app heard. No mouse required if you don't want one.

A small vibration on every press.
If your device supports the Vibration API (most Android phones do), every button press — touch or keyboard — gives a tiny 20 ms buzz. It's barely noticeable on its own, but it makes the calculator feel solid, like the keys are real.

Touch-first design.
The whole thing is sized to fit a phone screen without scrolling. Padding, gaps, and font sizes scale with the viewport. On a very short screen — a landscape phone, say — the subtitle disappears and the display tightens up, but everything else stays exactly where it was.

---

🧭 How it works

1. Open the file.
One HTML file. The calculator appears instantly, already in Minimalist Blue, ready to receive input. There's no splash, no setup, no tutorial.

2. Type or tap.
Use the on-screen keypad, or use your keyboard — numbers, operators, Enter, Backspace, Escape, %, all of it. The display fills with the expression above and the running result below.

3. Compute.
Press an operator, then another number, then = (or Enter). The result lands in the display, and the expression line shows what you just did. Press AC to clear everything and start fresh, or ⌫ to delete one digit.

4. Switch the mood, if you want.
Click SWITCH THEME in the header. The calculator cycles through the five designs. Nothing about your numbers changes — only the colours, fonts, and shapes. Your theme choice is not remembered between sessions.

5. Close the tab.
The calculator doesn't store anything, doesn't save history, doesn't remember what you last computed. Every session is a fresh session. Open it, use it, close it.

That's the whole app. No settings menu, no history panel, no memory keys, no scientific mode hiding somewhere behind a long-press.

---

🛠️ A few small helps

"Which theme am I in?"
You'll know by looking. But if you want to jump directly to a specific one, open the file in a text editor and change class="theme-1" on the <body> tag to theme-2, theme-3, theme-4, or theme-5. That theme becomes the starting one.

"Why isn't my theme saved?"
Because it isn't. Every visit starts at Minimalist Blue. This is deliberate — the app is meant to be opened, used for a moment, and closed. Saving a theme felt like the start of saving everything, and this is a calculator, not a profile.

"The operator buttons are coloured differently — is that on purpose?"
Yes. In every theme, the four arithmetic operators (÷ × − +) get the accent colour, and the function keys (AC, ⌫, %) get a distinct secondary colour. Numbers and the decimal point stay neutral. It's a small hierarchy that keeps your eye on the buttons that change the state of the calculation.

"Press 5, then ×, then = — what happens?"
You get 25. When you press = without entering a second operand, the calculator uses the first operand again. This matches how physical calculators behave, and it's genuinely useful for 5 × = to square a number quickly.

"Press 5, then ×, then + — what happens?"
It computes 5 × 5 = 25, shows you 25, and sets + as the pending operator. Chained operators always resolve the previous one first. Nothing is lost.

"Division by zero."
Shows Error in the display. Press AC to clear and continue. The = and other keys are ignored while in an error state, so you can't accidentally stack operations on top of the error.

"Why does the display change font size as I type?"
Longer numbers shrink to fit rather than getting clipped. There are three size tiers — normal, small, and tiny — and the display switches between them automatically. That's why the number seems to settle down as you get used to it.

"The thousand separators appear while I type — is that a problem?"
Not at all. The separators are only for display. The underlying number is stored as a plain string without commas, so calculations are unaffected.

"What's the largest number I can enter?"
Twelve digits by hand. After that, further digit presses are ignored — the display doesn't grow past what it can show cleanly. Results of calculations can be larger; they'll switch to exponential notation if they exceed 1e12.

"Can I use the numeric keypad on my keyboard?"
Yes. All number keys, including the ones on the numeric keypad, work. The operators on the numeric keypad work too. Enter and the numpad Enter both evaluate.

"Does it work offline?"
Yes. Once the file is open and the Google Fonts have loaded once, the entire calculator runs without the network. The math is all JavaScript, the display is all CSS, and nothing is sent anywhere.

"Why does the whole app vibrate when I press a key?"
If your device supports it, every press triggers a 20 ms vibration. If you find it distracting, you can either disable vibration for your browser in your phone's settings, or open the file and remove the vibrate() calls — there's a single function called vibrate() near the top of the script that you can simply empty.

"Can I add a sixth theme?"
Yes, if you're comfortable with CSS. Look at the block /* THEME 5: PINK POP-ART */ in the styles, copy that whole section, rename it theme-6, and adjust the colours and fonts. Then change const totalThemes = 5; to 6 near the top of the script, and the theme button will cycle through your new theme too.

"Why does the display overflow on my old phone?"
Very narrow screens — under 320 pixels — can push the display beyond its container. The app is designed for modern phones (375 px and up). On anything smaller, you may need to reduce the display font size in the .result CSS rule.

---

<div align="center">

📞 A question, an idea, a bug?

https://img.shields.io/badge/Email-mohamed005cheikh@gmail.com-d14836?style=flat-square&logo=gmail&logoColor=white
https://img.shields.io/badge/WhatsApp-+222_30_73_64_75-25D366?style=flat-square&logo=whatsapp&logoColor=white
https://img.shields.io/badge/GitHub-mohamed005cheikh--rgb-181717?style=flat-square&logo=github

<br />

Cinq humeurs. Une seule arithmétique.

<sub>© 2026 Mohamed Cheikh — MC88</sub>

</div>
