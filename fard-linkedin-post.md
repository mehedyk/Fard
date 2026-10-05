🔐 Shipping my first web project: Fard (فَرْد)

Fard is a password generator, but I didn't want to build "just another" one. A few things it does differently:

→ Real randomness. It uses the Web Crypto API (crypto.getRandomValues), not Math.random() — every character comes from the OS's own entropy source, not a predictable pseudo-random sequence.

→ Keeps a phrase intact. Drop in a word you'll actually remember, and Fard weaves random characters around it instead of forcing you to memorize total gibberish.

→ Live strength feedback. Every password gets scored in real time from length and character variety, so you're not guessing whether it's actually strong.

→ 100% client-side. No servers, no tracking, nothing ever leaves your browser.

Nothing about it is groundbreaking — it's a password generator — but it was a genuinely fun excuse to get hands-on with the Web Crypto API, entropy calculations, and building a UI I was actually happy with, all in plain HTML, CSS, and JavaScript.

Try it, break it, tell me what's missing:
🔗 Live demo: https://fard-pw.netlify.app/
💻 Source: https://github.com/mehedyk/Fard
🎬 Quick demo: https://youtube.com/shorts/ioFN8SVEZtE
📁 Project page: https://fusesw.vercel.app/projects/fard-password-generator

This is project #1. I'm going to keep building and posting as I go — appreciate any feedback along the way. 🙌

#webdev #javascript #buildinpublic #softwareengineering #100DaysOfCode #firstproject #cybersecurity
