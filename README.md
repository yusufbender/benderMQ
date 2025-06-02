# benderMQ
Modern, open-source MQTT client for exploring, publishing and analyzing MQTT traffic.

```markdown
# 🛰️ BenderMQ (MQTT Explorer Alternatifi)

BenderMQ, MQTT protokolü üzerinden veri alışverişini izleyebileceğin, canlı analiz yapabileceğin ve broker’la etkileşim kurabileceğin modern, web tabanlı bir MQTT aracı olarak geliştirilmiştir.

---

## 🚀 Özellikler (MVP)

- 🔌 MQTT Broker bağlantısı (TLS destekli)
- 📡 Topic’lere abone olma ve mesaj dinleme
- 🧾 Gelen mesajları canlı görüntüleme
- 📤 Mesaj gönderme
- 🌐 WebSocket ile anlık veri yayını

---

## 📂 Proje Yapısı

```
app/
├── main.py            # FastAPI başlangıç noktası
├── mqtt_client.py     # MQTT client bağlantı ve mesaj işleyici
├── websocket.py       # WebSocket bağlantı yöneticisi
├── config.py          # Ayarlar (.env üzerinden alınır)
```

---

## ⚙️ Kurulum

```bash
git clone https://github.com/yusufbender/bendermq.git
cd bendermq
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

---

## 📡 Çalıştırma

`.env` dosyasına broker bilgilerinizi girin:

```env
MQTT_HOST=broker.hivemq.com
MQTT_PORT=1883
MQTT_USER=
MQTT_PASSWORD=
```

Uygulamayı başlat:

```bash
uvicorn app.main:app --reload
```

---

## 🔭 Yol Haritası (Next Features)

- 🔒 TLS/SSL bağlantı desteği
- 🌲 Topic ağaç yapısı
- 📈 Anlık trafik grafiği
- 🧪 MQTT Simülatör (Test mesajları)
- 📁 JSON/XML/Base64 payload ayrıştırma
- 📤 Export & replay özelliği
```
