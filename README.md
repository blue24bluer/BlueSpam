# BlueSpam

[![Python](https://img.shields.io/badge/python-3.10+-blue)](https://www.python.org/)

BlueSpam is a Python-based spam tool created by **[@blue24bluer](https://github.com/blue24bluer)**. It allows sending automated requests/messages to a target phone number with support for proxies, Google Apps Script forwarding, custom user agents, and multi-threading.  

**Repository:** [bluespam](https://github.com/blue24bluer/bluespam)  
**Owner:** `blue24bluer`

---

## ⚡ Features

- Supports **custom User-Agents** for Android, iOS, and Dalvik.
- Optional **proxy support** (`HTTP/S`) for anonymity.
- Optional **Google Apps Script proxy** for request forwarding.
- Multi-threaded sending for faster execution.
- Adjustable **sleep intervals** between requests.
- Graceful handling of request errors.

---

## 📦 Requirements

- Python 3.10+
- Libraries:
  - `rich`
  - `requests`
  - `user_agent`

The script will attempt to install missing libraries automatically.

---

## 🛠️ Installation

1. Clone the repository:

```bash
git clone https://github.com/blue24bluer/bluespam.git
cd bluespam
````

2. Run the tool:

```bash
python3 BlueSpam.py --number +1234567890 --send 10
```

---

## 📝 Usage

```bash
python3 BlueSpam.py -n <target_number> -s <send_count> [options]
```

### Arguments

| Flag             | Description                                                                  |
| ---------------- | ---------------------------------------------------------------------------- |
| `-n, --number`   | Target phone number with country code (e.g., `+123456789`) **[Required]** |
| `-s, --send`     | Number of messages to send (default: 10)                                     |
| `--agent`        | Path to a file containing custom user agents (one per line)                  |
| `--sleep`        | Time to wait between requests in seconds (default: 1)                        |
| `-p, --proxy`    | Proxy to use for requests (e.g., `http://user:pass@127.0.0.1:8080`)          |
| `--google-proxy` | URL of a Google Apps Script proxy for forwarding requests                    |
| `-t, --threads`  | Number of concurrent threads (default: 1)                                    |

**⚠️ Note:** `--proxy` and `--google-proxy` cannot be used at the same time.

---

## 💡 Example

Send 50 messages to a target number using 5 threads:

```bash
python3 BlueSpam.py -n +123456789 -s 50 -t 5
```

Send messages using a proxy:

```bash
python3 BlueSpam.py -n +123456789 -s 20 -p http://127.0.0.1:8080
```

---

## 📌 Disclaimer

This tool is intended for **educational purposes only**. Misuse of BlueSpam for illegal spamming, harassment, or violating laws is strictly prohibited. The author is **not responsible** for any misuse.

---

## 🔗 Contact

* **Telegram:** [@Blue24Bluer](https://t.me/Blue24Bluer)
* **TikTok:** [@*blue24bluer*](https://www.tiktok.com/@_blue24bluer_)
* **Instagram:** [@*blue24bluer*](https://www.instagram.com/_blue24bluer_)
* **Discord:** Blue24Bluer#8271
* **Facebook:** Blu Bluer

```
