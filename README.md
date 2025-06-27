# 🔥 Restful-Booker API Performance Tests | JMeter

![JMeter](https://img.shields.io/badge/Apache_JMeter-5.6-red)
![Tests](https://img.shields.io/badge/Tests-8_passed-brightgreen)
![Reports](https://img.shields.io/badge/Reports-HTML_Dashboard-blue)
![License](https://img.shields.io/badge/License-MIT-green)

![Dashboard Preview](https://i.imgur.com/Jq5mG7p.png)

## 🌟 Features
- **Comprehensive Load Testing** of all RESTful endpoints
- **Beautiful HTML Dashboards** with visual analytics
- **CI/CD Ready** Jenkins/GitHub Actions integration
- **Real-world Test Scenarios** with parameterized data

## 🚀 Quick Start
```bash
# 1. Clone repository
git clone https://github.com/yourusername/restful-booker-performance-tests-jmeter.git

# 2. Run tests (Linux/Mac)
./run_tests.sh

# 3. View interactive report
open reports/dashboard/index.html

📊 Latest Results
Endpoint	Avg Latency	Throughput	Error Rate	90th %ile
🔐 Authentication	1631ms	0.61/s	0%	1631ms
➕ Create Booking	275ms	3.64/s	0%	275ms
🔍 Get Booking	281ms	3.56/s	0%	281ms
✏️ Update Booking	281ms	3.56/s	0%	281ms
🗑️ Delete Booking	282ms	3.55/s	0%	282ms
