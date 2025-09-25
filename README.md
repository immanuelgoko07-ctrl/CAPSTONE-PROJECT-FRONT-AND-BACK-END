# 🚗 AUTO AID – Smart Vehicle Maintenance Companion  
Table of contents

🚗 AUTO AID – Smart Vehicle Maintenance

✨ Features

🛠️ Tools & Technologies

📂 Project Structure

⚙️ Installation

🔑 API Keys

🚀 Usage

🌍 Deployment

🤝 Contributing

📜 License
## 📌 Project Description  
AUTO AID is a web-based platform designed to make car maintenance simple, affordable, and stress-free. It allows car owners to:
- Get **diagnostic suggestions** and **DIY guidance**.  
- Connect with **verified mechanics, repair shops, and genuine spare part suppliers**.  

By bridging the knowledge gap in car maintenance, AUTO AID prevents consumer exploitation, reduces roadside breakdowns, and contributes to safer roads.  

---

## ✨ Features   
- ✍️ Describe problems in text form.  
- 🔧 Get mechanic and shop recommendations.  
- 📍 Location-based mechanic/shop suggestions (Google Maps API integration).  
- 📊 Maintain a history of car problems and solutions.  
- 💡 DIY tutorials for minor issues.  
- 🔒 User authentication and profiles.  

---

## 🛠️ Tools & Technologies  
- **Backend**: Python (Flask/Django)  
- **Frontend**: HTML, CSS, Bootstrap, Jinja2 templates  
- **Database**: Firebase / PostgreSQL / MySQL  
- **Hosting/Deployment**: Lovable Studio, Firebase Hosting, GitHub Pages (where necessary)  
- **Other APIs**: Google Maps API (for shop/mechanic locations)  

---
USE CASE DIAGRAM
usecaseDiagram
  actor User
  actor Mechanic
  actor Admin

  rectangle "Auto Aid System" {
      User --> (Describe Car Problem)
      User --> (Upload Car Image/Video)
      User --> (Login / Authentication)
      User --> (Receive Suggested Solution)
      User --> (Find Nearby Mechanic)

      Mechanic --> (Register Shop/Service)
      Mechanic --> (Verify Profile)

      Admin --> (Verify Mechanics)
      Admin --> (Manage Database)
  }

  (Login / Authentication) --> (Firebase Auth)
  (Upload Car Image/Video) --> (Firebase Storage)
  (Describe Car Problem) --> (Flask Diagnosis Engine)
  (Find Nearby Mechanic) --> (Firestore Database)

 
## 🚀 Installation & Setup  

### 1. Clone the repository  
```bash
git clone https://github.com/your-username/auto-aid.git
cd auto-aid

VIRTUAL ENVIRONMENT
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

INSTALL DEPENDENCIES
pip install -r requirements.txt

APP RUNNING
python app.py

PROJECT STRUCTURE
AUTO-AID/
│── app.py                # Flask backend
│── requirements.txt       # Dependencies
│── static/                # Uploaded files, CSS, images
│── templates/             # HTML templates
│   ├── index.html
│   ├── recommend.html
│── README.md              # Project documentation

🎯 Objectives

Reduce road accidents caused by mechanical failures.

Save time and money for car owners.

Provide credible connections to verified mechanics and shops.

Create jobs and boost local economies.

Make car maintenance easy, cheap, and reliable.

🌍 Social Impact

Safer roads through timely maintenance.

Job creation for mechanics and local businesses.

Wider market access for spare part suppliers.

Globalization – connecting car owners and mechanics worldwide.

API KEY
<script src="https://maps.googleapis.com/maps/api/js?key={{ GOOGLE_MAPS_API_KEY }}&libraries=places"></script>
Usage
Visit: http://127.0.0.1:5000

Upload and find a mechanic.

Flash messages will confirm actions.
Deployment
Deploy on Lovable or Heroku.

For file storage in production → use Firebase Storage or Cloudinary instead of local /static/uploads.


























   

  
