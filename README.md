---

````md
# 🌌 NovaProxy  
### 🔒 Controlled Minecraft Proxy Infrastructure

> **Alle Verbindungen laufen ausschließlich über NovaProxy.**  
> Kein direkter Client-Kontakt, keine Drittanbieter, keine IP-Leaks.

---

## 🚀 Live Connection Flow

```text
[ Client ] 
    │
    │  join proxy.novaproxy.net
    ▼
[ NovaProxy ]
   🔍 Analyse
   🔐 IP-Isolation
   🧠 Routing
    ▼
[ Zielserver ]
````

```
⏳ CONNECTING
⬇
🔍 ANALYSING
⬇
🔐 MASKING IP
⬇
🚀 FORWARDING
⬇
✅ CONNECTED
```

---

## 🧠 Analyse Engine

NovaProxy verarbeitet **jede Verbindung intern**.

### 🔎 Was wird analysiert?

| Schritt          | Status | Beschreibung             |
| ---------------- | ------ | ------------------------ |
| 📥 Incoming      | ✅      | Client verbindet sich    |
| 🧠 Validation    | ✅      | Regeln & Zielprüfung     |
| 🔐 Privacy Layer | ✅      | Client-IP bleibt intern  |
| 📡 Forward       | ✅      | Verbindung über Proxy-IP |

```text
🧠 ANALYSE LOOP
├─ check client
├─ apply rules
├─ block direct access
└─ forward via proxy
```

---

## 🔐 IP-Isolierung (Core Feature)

```text
❌ Client → Zielserver
✅ Client → NovaProxy → Zielserver
```

🛡️ **Der Zielserver sieht nur:**

```
IP: NovaProxy
Client: unknown
```

🕶️ **Die echte Client-IP verlässt NovaProxy nie.**

---

## 🧱 Architektur

```text
┌──────────────┐
│  Spieler     │
│  (Client)    │
└──────┬───────┘
       │
       ▼
┌────────────────────┐
│   NovaProxy        │
│ 🔍 Analyse         │
│ 🔐 Privacy Layer   │
│ 🧠 Routing Engine  │
└──────┬─────────────┘
       │
       ▼
┌──────────────┐
│ Zielserver   │
│ (Minecraft)  │
└──────────────┘
```

---

## ⚙️ Features

* 🔒 **Volle IP-Abschirmung**
* 🧠 **Echtzeit-Analyse**
* 🧱 **Keine Direktverbindungen**
* 🌐 **Eigene Infrastruktur**
* ⚡ **Low-Latency Proxying**
* 🧩 **Modular erweiterbar**

---

## 🛠️ Konfiguration (Beispiel)

```yml
proxy:
  bind-ip: 0.0.0.0
  port: 25565

analysis:
  enabled: true
  log-level: full

privacy:
  hide-client-ip: true
  allow-direct: false

routing:
  type: internal
  target: mc.zielserver.net
```

---

## 📊 Status Animation (Markdown Style)

```
[■□□□□□□□□] Initializing
[■■□□□□□□□] Loading rules
[■■■□□□□□□] Starting analysis
[■■■■■□□□□] Binding ports
[■■■■■■■■■] Ready
```

---

## 🚨 Security Notes

✔ Keine Weitergabe an Dritte
✔ Kein externer Proxy / VPN
✔ Vollständig selbstverwaltet
✔ Kontrollierter Datenfluss

⚠️ **NovaProxy ist der einzige Verbindungspunkt.**

---

## 🗺️ Roadmap

```
[✔] Analyse Engine
[✔] IP Isolation
[✔] Internal Routing
[ ] Multi-Target Support
[ ] Auth Layer
[ ] Web Dashboard
[ ] Plugin API
```

---

## 🌌 Zusammenfassung

> **NovaProxy kontrolliert den gesamten Datenfluss.**
> Kein Umgehen. Kein Leaken. Kein Drittweg.

```
Client  →  NovaProxy  →  Server
```

---

## 📜 Lizenz

MIT License

```

---

Wenn du willst, mache ich dir als Nächstes:
- 🎨 **richtiges ASCII-Logo**
- 🧑‍💻 **Ultra-technische Dev-README**
- 🧾 **Privacy / DSGVO-Abschnitt**
- 🔥 **GitHub-optimierte README mit Badges**

Sag einfach was 🔥
```
