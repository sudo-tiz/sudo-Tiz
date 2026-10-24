<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1b26,100:7aa2f7&height=120&section=header" />
  <h1>sudo-Tiz — The Immutable Zero</h1>
  <p>Systems & DevSecOps · Arch Linux · Hyprland · Go · Python · Ansible</p>
  <p>
    <img src="https://img.shields.io/badge/Arch_Linux-black?logo=archlinux&logoColor=white" />
    <img src="https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white" />
    <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white" />
    <img src="https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white" />
    <img src="https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white" />
    <img src="https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white" />
    <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/Rust-black?logo=rust&logoColor=white" />
  </p>
</div>

## About

Systems & DevSecOps — building infrastructure that is automated,
observable and secure by default.

DNS & NTP, CI/CD, observability, infrastructure as code on a Linux base.
Cyber-security background; Go, Python and shell when the tool doesn't exist yet.

## Stack

| | |
|---|---|
| IaC & CI/CD | Ansible · Terraform · GitLab CI · ArgoCD · Helm · Renovate · Trivy · Vault |
| Containers | Docker · Kubernetes · Traefik · Nginx |
| Network & DNS | PowerDNS · Bind · Unbound · NTP · WireGuard · nftables |
| Observability | Prometheus · Grafana · Loki · Alloy · Alertmanager |
| Security | Fail2ban · CIS-CAT · Trivy · mobile/web/API pentesting · Frida |
| Languages | Go · Python · Shell · Kotlin · Rust · Lua |
| Systems | Arch · Debian · Ubuntu · Proxmox |

## Self-hosting

One `justfile`, one shared inventory, two playbooks:

```
server                     just + shared inventory
 ├─ mash-playbook            services: Docker, Traefik, PostgreSQL, borg…
 └─ math-playbook            host setup, firewall, mail relay, APT, KVM VMs
```

| | |
|---|---|
| [server](https://github.com/sudo-Tiz/server) | Entry point: syncs the inventory, then runs MASH or math |
| [math-playbook](https://github.com/sudo-Tiz/math-playbook) | Idempotent Ansible roles for what MASH doesn't cover (Debian family) |
| [mash-playbook](https://github.com/mother-of-all-self-hosting/mash-playbook) | Upstream MASH, used unmodified |

## Config

| | |
|---|---|
| [LARBRE](https://github.com/sudo-Tiz/LARBRE) | Arch Linux auto-setup: one script → Hyprland desktop, dotfiles, secure DNS |
| [fast_linux_config](https://github.com/sudo-Tiz/fast_linux_config) | Minimal dotfiles for a fresh Linux box (Neovim, Tmux, Zsh, Bash) |

## Projects

| | |
|---|---|
| [Duper](https://github.com/sudo-Tiz/Duper) | Lost your phone? Send it "duper" — Android tracker over SMS, no internet. Kotlin, on F-Droid |
| [dns-tester-go](https://github.com/sudo-Tiz/dns-tester-go) | DNS testing tool for UDP, TCP, DoT, DoH and DoQ |
| [asus-numpad](https://github.com/sudo-Tiz/asus-numpad) | Lightweight Go driver for Asus touchpad-integrated numpads |
| [fridapk](https://github.com/sudo-Tiz/fridapk) | Inject Frida Gadget into Android APKs, no root |

## Contributions

- [mash-playbook](https://github.com/mother-of-all-self-hosting/mash-playbook) — merged roles & services: Lidarr, Bazarr, Jellyseerr, FlareSolverr, Endlessh-go, LanguageTool, plus ansible-role-loki/-nextcloud/-grafana/-qbittorrent fixes
- [Tsumiki](https://github.com/rubiin/Tsumiki) (Python) · [Ashell](https://github.com/MalpenZibo/ashell) (Rust)
