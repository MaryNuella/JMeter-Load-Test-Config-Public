- # JMeter Load Test Config

This repository contains JMeter test plans and supporting files used for performance and load testing of APIs and services.  
The goal is to validate response times, error rates, and system behavior under expected and peak load conditions.

---


---

## 🚀 Getting Started

### Prerequisites
- [Apache JMeter 5.6+](https://jmeter.apache.org/download_jmeter.cgi) installed  
- Java 8 or higher installed (`java -version` to confirm)  

### Run a Test in GUI Mode
```bash
jmeter -t tests/login_flow.jmx

Run a Test in CLI Mode (non-GUI, recommended for load tests)
jmeter -n -t tests/login_flow.jmx -l results/test_results.jtl -e -o results/dashboard

-n → Non-GUI mode

-t → Path to the test plan (.jmx)

-l → Log results to a .jtl file

-e -o → Generate an HTML dashboard report


 ## After execution, open the dashboard in your browser:

results/dashboard/index.html



📊 Reports

Summary Report: Response times, error %, throughput

HTML Dashboard: Detailed graphs of latency, percentiles (90th, 95th, 99th), and errors


👩🏽‍💻 Author

Maintained by MaryNuella – QA Engineer passionate about performance testing and automation.
