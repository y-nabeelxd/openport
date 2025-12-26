# OpenPort

OpenPort is a powerful yet simple Linux firewall management tool.
It allows you to open, close, list, manage, and **uninstall** firewall rules easily using human‑friendly commands.

---

## 🚀 One‑Line Installation

```bash
curl -sSL https://nabeelxd.vercel.app/openport-installer | sudo bash
```

---

## 📦 Installed Commands

- `openport` – Open, manage, or uninstall firewall rules
- `closeport` – Close opened ports
- `listports` – List current firewall rules

---

## 🧑‍💻 Usage Examples

### Open a port
```bash
openport 80
```

### Open a range
```bash
openport 8000-8010
```

### UDP port
```bash
openport 53 --udp
```

### Allow only one IP
```bash
openport 22 --from=192.168.1.10
```

### IPv6 support
```bash
openport 443 --ipv6
```

### Close ports
```bash
closeport 80
closeport 8000-8010
```

### List ports
```bash
listports
```

---

## 🧪 Safe Testing (Dry‑Run)

```bash
openport 80 --dry-run
```

No firewall changes are applied.

---

## 🧹 Delete All Firewall Rules

```bash
openport --delete-all
```

> ⚠️ This resets the firewall completely.

---

## 🗑️ Uninstall OpenPort

```bash
sudo openport --uninstall
```

This removes:
- `openport`
- `closeport`
- `listports`
 
No firewall rules are modified during uninstall.

---

## 📊 Firewall Status

```bash
openport status
```

---

## 🆘 Help Menu

```bash
openport --help
closeport --help
listports --help
```

---

## 🔥 Supported Firewalls

- UFW (Ubuntu / Debian)
- Firewalld (CentOS / RHEL / Alma / Rocky)

Auto‑detected.

---

## ⚠️ Security Note

Only open ports you really need.
Unused open ports are security risks.

---

## 📜 License

MIT License
