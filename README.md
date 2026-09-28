# example-content

An example [Tico](https://tico.team) bot that plans and drafts a company's posts and articles and
hands each one over for a person to publish. It keeps a rolling plan, a list of unwritten ideas, and a
description of how the company sounds. It never publishes, schedules, posts, or replies anywhere, and
it never invents a number, quote, or result.

Examples use a fictional company, Acme Co (`acme.example`). Replace them.

## What it needs

- Read access to your own published content and the sources you want cited (the web is enough).
- Nothing that writes to a channel. No social, CMS, or newsletter credentials.

## What it must never do

- Publish, schedule, post, comment, or reply on any channel.
- Change live copy on the website.
- Invent a number, a customer quote, or a result. Every claim carries a dated source.

## Add it to a Tico install

1. Create `<your-org>/emp-content` from this template (`gh repo create --template ticoteam/example-content`).
2. Write `knowledge/voice.md` and `knowledge/company.md` for real. The bot is only as good as these.
3. Ask BotOps to set up a content bot from that repository. It registers the bot and runs
   `hub bot check content`. The bot stays `planned` until you activate it.

## Customize

- `knowledge/voice.md`: how you sound, with three real sentences you would and would not write.
- `knowledge/plan.md` and `knowledge/ideas.md`: what is planned and what is waiting.
- `playbooks/`: add a playbook per format (a newsletter, a changelog post) as you use them.
- `employee.yaml`: runtime and model (your install chooses), and an optional weekly planning routine.

## Contributing

Pull requests welcome: better editing checks, format playbooks, generic voice guidance. Keep
contributions generic: no real company names, quotes, domains, or credentials; use Acme.

## License

Apache-2.0. See `LICENSE`.
