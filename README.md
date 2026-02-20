# 📡 WebRTC Signaling Server – Backend

This is the signaling server used for the WebRTC video calling application.

Live Server:
https://webrtc-video-backend-hbnb.onrender.com

---

## 🚀 Tech Stack

- Node.js
- Express
- Socket.IO
- Render (Deployment)

---

## 📡 What is Signaling?

WebRTC cannot automatically connect two peers.

Before direct communication happens, browsers must exchange:

- SDP Offer
- SDP Answer
- ICE Candidates

This exchange process is called Signaling.

This server handles that process using Socket.IO.

Once peers connect, media does NOT pass through this server.

---

## 🔄 Connection Flow

1. User joins a room.
2. Server notifies other peer.
3. Offer is sent.
4. Answer is returned.
5. ICE candidates exchanged.
6. Peer-to-peer connection established.

---

## 🛠 Run Locally

```bash
npm install
node server.js
```

---

## 🌍 Deployment Notes

- Enable CORS properly
- Use HTTPS in production
- Render free tier may sleep after inactivity

---

## 👨‍💻 Author

<p align="center">
  <img src="https://github.com/Balakrishnamoorthy.png" width="150" style="border-radius:50%" />
</p>

<p align="center">
  <b>Balakrishnamoorthy</b>
</p>

<p align="center">
<a href="https://github.com/Balakrishnamoorthy">
    <img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github" />
  </a>
  <a href="https://balakrishnamoorthy-portfolio.netlify.app/">
    <img src="https://img.shields.io/badge/Portfolio-111?style=for-the-badge" />
  </a>
</p>
