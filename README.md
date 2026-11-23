
```markdown
# SkyGuard AI: Real-Time Flood Risk Assessment & Alerting App

SkyGuard AI is a lightweight, cloud-integrated Streamlit web application designed to help rural communities in Pakistan monitor local flood risks and receive automated multilingual alert SMS notifications.

## 🚀 Features
…```

## 🛡️ Ethics & Privacy Note
* **Informational Purposes Only:** This app utilizes open-source AI analysis and public satellite data. For critical emergencies, always verify with official agencies (NDMA/PMD).
* **Data Privacy:** This app is stateless and does not record personal coordinates or mobile numbers.
```
# SkyGuard AI: Real-Time Flood Risk Assessment & Alerting App

SkyGuard AI is a lightweight, cloud-integrated Streamlit web application designed to help rural communities in Pakistan monitor local flood risks and receive automated multilingual alert SMS notifications.

## 🚀 Features
- **Real-Time Rainfall Monitoring:** Fetches Earth Engine precipitation data (NASA IMERG) for live verification.
- **Soil Moisture Conditions:** Retrieves current telemetry stats from ThingSpeak public sensors.
- **Official Policy Tracking:** Scrapes the latest bulletins and reports from the National Disaster Management Authority (NDMA) and Pakistan Meteorological Department (PMD).
- **Automated AI Risk Classification:** Uses a dedicated Climate Attitude Language Model (`KevSun/climate-attitude-LM`) to classify hazard severity (High, Medium, Low).
- **Multilingual Alerts:** Auto-translates action plans to Urdu for local accessibility using `deep-translator`.
- **SMS Notifications:** Sends instant emergency SMS alerts via Twilio.
- **Interactive Mapping:** Pinpoints exact coordinates on a visual Leaflet map (via Folium).

## 🛠️ Local Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/skyguard-ai.git
cd skyguard-ai
2. Install dependencies
pip install streamlit twilio folium streamlit-folium transformers torch earthengine-api requests beautifulsoup4 deep-translator python-dotenv
3. Configure Environments & Secrets
Create a .env file or set up Streamlit Secrets (.streamlit/secrets.toml):

TWILIO_SID=your_twilio_sid
TWILIO_TOKEN=your_twilio_auth_token
TWILIO_NUMBER=your_twilio_phone_number
EE_PROJECT_ID=your_gee_project_id
HF_TOKEN=your_huggingface_write_token
4. Run the App
streamlit run app.py
🛡️ Ethics & Privacy Note
Informational Purposes Only: This app utilizes open-source AI analysis and public satellite data. For critical emergencies, always verify with official agencies (NDMA/PMD).
Data Privacy: This app is stateless and does not record personal coordinates or mobile numbers.
