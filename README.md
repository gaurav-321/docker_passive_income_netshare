# Passive Income Docker Stack

This Docker Compose stack lets you run multiple passive income applications simultaneously on your server or VPS. Each container connects to a platform that pays users for sharing bandwidth or device resources.

The stack includes auto-update functionality using Watchtower.

---

## 🚀 Getting Started

### 1. Clone this repository:
```bash
git clone https://github.com/yourusername/passive-income-docker.git
cd passive-income-docker
```

### 2. Update Your Credentials:
Edit `docker-compose.yml` and replace placeholders with your actual credentials.
You must change email addresses, passwords, API keys, UUIDs, and tokens as indicated by the comments.

You can optionally include your referral links in the comments.

### 3. Start the Containers:
```bash
docker compose up -d
```

---

## 📦 Services Included

### 1. Honeygain  
**[Sign Up](https://r.honeygain.me/GAURA57077)**  
**What it does:** Share your unused internet bandwidth.  
**Required changes:** Replace email, password, and optionally the device name.
```yaml
-email your_email@example.com
-pass your_password
-device ubuntu_server1
```

---

### 2. EarnApp  
**[Sign Up](https://earnapp.com/i/etWBlbZw)**  
**What it does:** Earn by sharing bandwidth through secure proxy nodes.  
**Required changes:** Replace the `EARNAPP_UUID` with your unique EarnApp UUID.
```yaml
- EARNAPP_UUID=your_uuid_here
```

---

### 3. PacketStream  
**[Sign Up](https://packetstream.io/?psr=6KN0)**  
**What it does:** Earn money by becoming a residential proxy node.  
**Required changes:** Replace the `CID` with your personal Client ID.
```yaml
- CID=your_cid_here
```



---

### 4. IPRoyal Pawns  
**[Sign Up](https://pawns.app/?r=4301760)**  
**What it does:** Share bandwidth and get paid.  
**Required changes:** Replace email and password.
```yaml
-email=your_email@example.com
-password=your_password
```

---

### 5. EarnFM  
**[Sign Up](https://earn.fm/ref/PYTHJYM9)**  
**What it does:** Earn money by streaming content/audio.  
**Required changes:** Replace the `EARNFM_TOKEN` with your valid token.
```yaml
- EARNFM_TOKEN=your_token_here
```

---

### 6. Repocket  
**[Sign Up](https://link.repocket.com/YDmQ)**  
**What it does:** Share residential IP and earn money.  
**Required changes:** Replace email and API key.
```yaml
- RP_EMAIL=your_email@example.com
- RP_API_KEY=your_api_key_here
```

---

### 7. Traffmonetizer  
**[Sign Up](https://traffmonetizer.com/?aff=1693337)**  
**What it does:** Share bandwidth to earn passive income.  
**Required changes:** Replace the `--token` value with your Traffmonetizer token.
```yaml
command: start accept --token your_token_here
```
---

# Watchtower
**What it does:** Automatically updates all running containers to the latest image versions.  
**Required changes:** None, fully configured.

