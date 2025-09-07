# grug

> *"complexity very bad" - grug*

A monorepo for Stellar blockchain dApps built with Go, HTML, and CSS. No framework magic. No npm madness. Just simple tools that work even in w3m and links browsers.

Built for Montelibero and Programmers Guild DAOs. Because grug know: simple tools make happy developer.

## What This Is

grug is collection of simple web applications for Stellar blockchain:
- **No JavaScript frameworks** - grug no need React for display text
- **Single binaries** - deploy like caveman: copy file, run file
- **Works everywhere** - even in terminal browser (w3m/links compatible)
- **Go + HTML + CSS** - tools grug understand, tools that last forever

## What This Is NOT

- ❌ Not another "modern" web3 dApp with 500MB of node_modules
- ❌ Not requiring webpack, babel, or other complexity demons
- ❌ Not chasing latest framework fashion trends
- ❌ Not making simple things complex

grug say: "complexity demon say 'you need this for scale' but grug notice scale never come"

## Project Structure

```
grug/
├── apps/           # Web applications with frontend
│   ├── crowd/      # Crowdfunding for projects
│   ├── miskdao/    # Miskatonic Club DAO (prediction markets)
│   ├── notary/     # Document notarization as NFTs
│   └── social/     # Social connections via soulbound tokens
├── pkgs/           # Shared Go modules
├── cmd/            # CLI utilities
├── templates/      # HTML templates for reuse
└── assets/         # CSS, minimal JS for sharing
```

## Grug Philosophy Applied

### 1. Complexity Very Bad
Every line of code is line that can break. grug use Go standard library when possible. Echo for web because simple. No ORM - SQL is fine. No GraphQL - REST is fine.

### 2. Say No to Shiny
New JavaScript framework come out every moon cycle. grug ignore. HTML work for 30 years, will work for 30 more. CSS is enough for pretty. Native JS only when absolutely needed.

### 3. Test Like Grug Test Rock
Rock either break or not break. Test either pass or not pass. Use testify for simple assertions. Use mockery for mocks. No BDD. No complexity testing framework.

### 4. Deploy Like Throw Spear
Build single binary. Copy to server. Run. No Docker if not needed. No Kubernetes for one app. systemd is friend - been around since before grug, will be around after.

### 5. Frontend No Need Big Brain
- html/template for rendering
- Embedded assets with `embed`
- Forms work fine without JavaScript
- Progressive enhancement only where needed
- If work in w3m, work everywhere

## Tech Stack

- **Language**: Go (standard library + minimal dependencies)
- **Web Framework**: Echo (simple routing, middleware)
- **Templates**: html/template
- **Blockchain**: Stellar via github.com/stellar/go
- **Testing**: testify + mockery
- **Database**: PostgreSQL (probably, grug like elephant)
- **Assets**: Embedded with Go's `embed` package

## Getting Started

```bash
# grug clone repo
git clone https://github.com/yourusername/grug.git
cd grug

# grug get dependencies
go mod download

# grug run app
cd apps/crowd
go run .

# grug build for production
go build -o crowd .
./crowd

# grug deploy (copy binary to server and run)
scp crowd server:/usr/local/bin/
ssh server 'systemctl restart crowd'
```

## Development Principles

1. **Prefer Boring Technology** - PostgreSQL over fancy NoSQL. HTML forms over SPA.
2. **No Build Steps** - Go binary include everything. No "npm run build".
3. **Accessibility First** - If blind developer with screen reader can use, grug happy.
4. **URLs Are UI** - /user/123 better than /#/app/user?id=123
5. **HTML First, JavaScript Last** - Form submission work without JS. Add JS only for enhance.

## Apps Overview

`TODO`

## Contributing

grug welcome help from other grugs!

1. **Issues First** - Before code, create issue. Discuss. Agree on approach.
2. **Simple PR** - One thing per PR. Easy review. Easy revert if needed.
3. **Test Your Rock** - Add test. Run `go test ./...`. Make sure rock solid.
4. **No Clever** - Clever code is bad code. Write boring code.

```bash
# grug way to contribute
1. Fork repo
2. Create branch: git checkout -b grug-fix-thing
3. Make changes (keep simple!)
4. Test: go test ./...
5. Commit: git commit -m "fix: thing was broken, now not broken"
6. Push: git push origin grug-fix-thing
7. Open PR with good description
```

## Why This Approach?

Modern web development has complexity disease. 200 dependencies to display text. 50MB JavaScript bundle to show form. GraphQL to fetch three fields. Kubernetes to run blog.

grug see this and think: "why?"

Stellar blockchain is simple. Go is simple. HTML is simple. When combine simple things in simple way, get powerful result without complexity demon.

This project proof that can build real Web3 applications without modern web complexity. Work in terminal browser is not limitation - is proof of simplicity.

## Requirements

- Go 1.21+ (for good embed support)
- PostgreSQL 14+ (or SQLite for development)
- Stellar testnet/mainnet account
- Brain (preferably grug-sized)

## License

MIT - because grug believe in simple license too

## Contact

- Programmers Guild DAO: [mtlprog.xyz](https://mtlprog.xyz)
- Montelibero: [montelibero.org](https://montelibero.org)
- Issues: Use GitHub issues
- PRs: Welcome, but issue first!

---

*"grug wonder why big brain take hardest path up mountain. grug take easy path. both reach top of mountain."*
