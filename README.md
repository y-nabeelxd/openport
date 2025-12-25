# OpenPort

OpenPort is a powerful yet simple Linux firewall management tool.
It allows you to open, close, list, and manage firewall ports easily using human‑friendly commands.

---

## 🚀 One‑Line Installation

```
sudo bash <(curl -sSL https://nabeelxd.vercel.app/openport-installer)
```

---

## 📦 Installed Commands

- `openport` – Open firewall ports
- `closeport` – Close firewall ports
- `listports` – List current firewall rules

---

## 🧑‍💻 Usage Examples

### Open a port
```
openport 80
```

### Open a range
```
openport 8000-8010
```

### UDP port
```
openport 53 --udp
```

### Allow only one IP
```
openport 22 --from=192.168.1.10
```

### IPv6 support
```
openport 443 --ipv6
```

### Close ports
```
closeport 80
closeport 8000-8010
```

### List ports
```
listports
```

---

## 🧪 Safe Testing (Dry‑Run)

```
openport 80 --dry-run
```

No firewall changes are applied.

---

## 🧹 Delete All Firewall Rules

```
openport --delete-all
```

> ⚠️ This resets the firewall completely.

---

## 📊 Firewall Status

```
openport status
```

---

## 🆘 Help Menu

```
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
