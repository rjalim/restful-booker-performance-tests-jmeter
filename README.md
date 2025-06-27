# 🔥 Restful-Booker API Performance Tests | JMeter

![JMeter](https://img.shields.io/badge/Apache_JMeter-5.6-red)
![Tests](https://img.shields.io/badge/Tests-8_passed-brightgreen)
![Reports](https://img.shields.io/badge/Reports-HTML_Dashboard-blue)
![License](https://img.shields.io/badge/License-MIT-green)

![Dashboard Preview](reports/dashboard/preview.png)

## 🌟 Features
- **Comprehensive Load Testing** of all RESTful endpoints
- **Beautiful HTML Dashboards** with visual analytics
- **CI/CD Ready** (Jenkins / GitHub Actions integration possible)
- **Real-world Test Scenarios** with parameterized data

---

## 🚀 Quick Start
```bash
# 1. Clone repository
git clone https://github.com/MD-Abdul-Alim/restful-booker-performance-tests-jmeter.git

# 2. Run tests (Linux/Mac example)
./run_tests.sh

# 3. View interactive report
open reports/dashboard/index.html
📊 Latest Results
Endpoint	Avg Latency	Throughput	Error Rate	90th Percentile
🔐 Authentication	1631ms	0.61/s	0%	1631ms
➕ Create Booking	275ms	3.64/s	0%	275ms
🔍 Get Booking	281ms	3.56/s	0%	281ms
✏️ Update Booking	281ms	3.56/s	0%	281ms
🗑️ Delete Booking	282ms	3.55/s	0%	282ms

📈 Request Distribution
mermaid
Copy
Edit
pie showTitle
    title Request Distribution
    "Auth" : 15
    "Create" : 20
    "Read" : 25
    "Update" : 20
    "Delete" : 20
🏗️ Project Structure
graphql
Copy
Edit
restful-booker-performance-tests-jmeter/
├── test-plans/          # JMeter test scripts (.jmx)
├── test-data/           # Parameterization CSVs
├── results/             # Raw results (.jtl, .json)
├── reports/             # HTML dashboards
│   └── dashboard/       # Interactive visualizations
├── config/              # Environment properties
└── scripts/             # Execution helpers
🛠️ Customization Guide
🔧 Modify Test Load
xml
Copy
Edit
<!-- Inside your .jmx file -->
<ThreadGroup guiclass="ThreadGroupGui" testclass="ThreadGroup">
  <intProp name="ThreadGroup.num_threads">100</intProp> <!-- Virtual Users -->
  <intProp name="ThreadGroup.ramp_time">300</intProp>  <!-- Ramp-up time -->
</ThreadGroup>
📊 Generate Comparative Reports
bash
Copy
Edit
jmeter -g results/*.jtl -o reports/compare/ --jmeterproperty reportgenerator.comparison_keys=Label,Avg,Error%
💡 Pro Tips
Spot performance bottlenecks in reports/dashboard/statistics.json

Compare runs using the --compare flag

Automate testing via GitHub Actions or Jenkins

📜 License
MIT © 2025 MD. Abdul Alim
Made with ❤️ using Apache JMeter | Last run: 2025-06-27
