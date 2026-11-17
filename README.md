# The Quant Observatory

Original fixed exercises, tests, quizzes and interactive experiments for probability, decisions, market making, research and programming. No model calls or paid API key. Progress stays in the browser and supports export/import. Exercises are original and are not claimed to be actual interview questions.

Teaching design adapts [Jane Street’s Socratic Tutor skill](https://github.com/janestreet/agent_skills), with the [MIT notice](public/licenses/jane-street-socratic-tutor.txt). Independent, without Jane Street endorsement; the notice does not license the application or original curriculum.

Website: https://thequantobservatory.com/ . Conversational companion: https://thethinkingobservatory.com/ . Courses: https://tglauner.com/#courses .

```bash
npm ci
npm run check
npm run dev
```

Open http://127.0.0.1:5173/ . Stop with Control-C. If the tutor preview is using that port, stop it first.

```bash
npx cf auth login
npm run deploy
curl -I https://thequantobservatory.com/
```

The pinned cf CLI deploys only the explicit dist/ allowlist as Worker `thequantobservatory`, on the apex and www hostnames. No database or model service. Check lessons, diagnostic, assessment, lab, saved progress and course links after deployment. Roll back using the previous Worker version in Cloudflare’s Deployments page.
