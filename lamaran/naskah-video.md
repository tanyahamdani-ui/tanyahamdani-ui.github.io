# Naskah video & bahan wawancara

Tips rekam: pakai QuickTime (File → New Screen Recording / Movie Recording) atau Loom gratis. Bicara pelan, tidak perlu hafal — baca sambil sesekali lihat kamera. Unggah ke YouTube (Unlisted) atau Loom, lalu tempel link-nya di form QuickMail.

---

## Video 1 — QuickMail: "SPF, DKIM, dan DMARC untuk pelanggan awam" (±3 menit)

Hi, I'm Dani. I'll explain three email settings, SPF, DKIM and DMARC, without the technical jargon.

Think of sending an email like sending a letter from your company. The person receiving it wants to know two things: did this letter really come from you, and was it changed on the way? These three settings answer those questions.

First, SPF. SPF is a public list that says: "These are the post offices allowed to send mail for my company." When your email arrives, the receiving server checks the list. If the email came from a sender on the list, good. If it came from somewhere else, it looks suspicious. So if you start sending through a new tool, like QuickMail, that tool needs to be added to your list.

Second, DKIM. DKIM is like a wax seal on the envelope. Your sending service signs every email with a private key, and the receiver checks the signature with a public key you publish. If the seal is intact, the receiver knows the message really came from your domain and wasn't changed on the way.

Third, DMARC. DMARC is your instruction to the receiver: "If an email claims to be from me but fails SPF and DKIM, here is what to do with it." You can say "just report it to me," "put it in spam," or "reject it." It also sends you reports, so you can see who is sending email using your name.

Why does this matter for you? Without these three, inbox providers like Gmail and Outlook can't trust your emails, so more of them land in spam. That means fewer replies and fewer leads. With all three set up correctly, your emails look trustworthy, and your campaigns reach the inbox.

The good news: you set these up once, by adding a few records in your domain settings. I can walk you through it step by step, and we can check together that everything passes before you send your next campaign.

Thanks for watching.

---

## Video 2 — QuickMail: "Kapan eskalasi ke developer, kapan terus menggali" (±3 menit)

Hi, I'm Dani. I spent more than ten years in telecom network operations, where deciding when to escalate was part of the job every day. Here's how I decide.

First, I reproduce the problem. If I can't reproduce it, I collect more facts from the customer: what they did, when it happened, screenshots, the account and campaign IDs. Most issues get clearer at this step.

Second, I check the known causes. Is it a setting, a DNS record, a limit on the customer's email provider, or something already in our help docs? If it's a known cause, I keep digging and solve it myself, because escalating would only slow the customer down.

Third, I look at impact and time. I escalate quickly when many customers are affected, when data might be lost or sent to the wrong people, or when the customer's business is blocked right now. In those cases, speed matters more than me finding the root cause alone.

Fourth, I escalate when the evidence points to our product: the app behaves differently from the documentation, the logs show an error on our side, or I can reproduce a bug with clear steps.

When I do escalate, I make it easy for the developer: a short summary, steps to reproduce, what I already checked, the affected accounts, and how urgent it is. A good escalation saves the developer time instead of handing them a mystery.

And I keep the customer informed the whole time, with honest updates, even when the update is "we're still investigating."

So my rule is simple: dig until the evidence points to the product or the impact is too big to wait, then escalate with everything the developer needs.

Thanks for watching.

---

## Askable — wawancara rekaman 10 menit (bahan jawaban)

Kemungkinan pertanyaan dan poin jawabannya (jawab dengan kalimatmu sendiri):

1. **Tell us about yourself.** 10+ years telecom network operations (NOC, since 2012). Built and run Kelola.in alone: JavaScript PWA on Supabase Postgres, 21 Deno/TypeScript Edge Functions, LLM features, OAuth integrations. Also ~150 Node.js scripts and 46 scheduled jobs automating my perfume brand.
2. **A codebase you know well (untuk tugas mereka).** Kelola.in — private codebase I own. Example change: the server-side AI proxy with quota and model fallback, or the content calendar view in Studio.
3. **How do you test your work?** Syntax checks and builds before deploy, testing in the browser on desktop and mobile, checking the live site after deploy, and validating AI output (reject malformed JSON and retry).
4. **Experience with AI models.** I use Claude and Gemini daily, both as coding assistants and inside my product. I review generated code instead of trusting it.
5. **Professional experience requirement (2+ years).** Be honest: "My professional title was network operations engineer for 10+ years; my software work is on products I built and own."
6. **Availability.** Part-time, about 10 hours a week, evenings and weekends Jakarta time.

Siapkan: CV PDF (Desktop/portfolio-hamdani/CV-Hamdani-Nur-Arifin.pdf), kamera, mikrofon, tempat tenang.
