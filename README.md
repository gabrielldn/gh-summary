<p align="center">
  <a href="https://github.com/gabrielldn/gh-summary/stargazers">
    <img src="https://img.shields.io/github/stars/gabrielldn/gh-summary" alt="GitHub stars">
  </a>
  <a href="https://github.com/gabrielldn/gh-summary/network/members">
    <img src="https://img.shields.io/github/forks/gabrielldn/gh-summary" alt="GitHub forks">
  </a>
  <a href="https://github.com/gabrielldn/gh-summary/issues">
    <img src="https://img.shields.io/github/issues/gabrielldn/gh-summary" alt="GitHub issues">
  </a>
  <a href="https://github.com/gabrielldn/gh-summary/issues-pr">
    <img src="https://img.shields.io/github/issues-pr/gabrielldn/gh-summary" alt="GitHub PR">
  </a>
  <img src="https://img.shields.io/github/license/gabrielldn/gh-summary" alt="MIT license">
</p>

<h1 align="center">gh-summary</h1>
<p align="center">
  A minimal <strong>GitHub CLI</strong> extension that gives you a terminal snapshot of your daily activity:<br>
  commits, lines, characters & contribution graph count.
</p>


## ✨ Why use it?

- **Quick feedback** – Instantly see your daily contribution stats without opening GitHub in the browser.
- **Gamify your coding** – Compare activity with friends (responsibly, no commit spamming 😄).
- **Detailed insight** – View number of lines added, removed, and even character count.
- **Terminal-friendly** – Stay in the terminal while checking your GitHub productivity.

If you like seeing numbers and progress, you're not alone — this tool exists exactly for that reason.

---

## 🚀 Features

| Metric             | Source                             |
|--------------------|------------------------------------|
| Commits            | `gh search commits`                |
| Lines & Characters | GitHub REST API (commit details)   |
| Contributions      | GitHub GraphQL API (calendar data) |

All heavy lifting happens locally with Bash + `jq`; the only requirement is the official [GitHub CLI](https://cli.github.com/).

---

## 📦 Installation

> **Pre-requisite:** GitHub CLI (`gh`) installed and authenticated via `gh auth login`.

### Install

```bash
gh extension install gabrielldn/gh-summary
````

### Update

```bash
gh extension upgrade gh-summary
```

### Remove

```bash
gh extension remove gh-summary
```

List installed extensions:

```bash
gh extension list
```

---

## 🖥️ Usage

```bash
# Show summary for today
gh summary

# Show summary for another user
gh summary --author torvalds

# Show summary for a specific date (UTC)
gh summary --author-date 2025-07-18
```

Example output:

```
╔════════════════════════╗
║ Summary for 2025-07-18 ║
╠────────────────────────╣
║ Commits            5   ║
║ Total lines       264  ║
║ Characters       9668  ║
║ Contributions      7   ║
╚════════════════════════╝
```

---

## 🗺️ Roadmap

* [ ] To be discussed

---

## 🤝 Contributing

Anyone is welcome to collaborate!

* Fork the repo
* Make your changes in a branch
* Use [Conventional Commits](https://www.conventionalcommits.org)
* Open a pull request

If you like this project, feel free to ⭐ it and share with friends.

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 🧰 About GitHub CLI

> `gh` is GitHub on the command line. It brings pull requests, issues and other GitHub concepts to your terminal next to where you're already working with `git`.

![GitHub CLI Screenshot](https://user-images.githubusercontent.com/98482/84171218-327e7a80-aa40-11ea-8cd1-5177fc2d0e72.png)

GitHub CLI works on macOS, Windows, and Linux — supporting GitHub.com, Enterprise Cloud, and Server 2.20+.

For full documentation, visit: [cli.github.com](https://cli.github.com)
