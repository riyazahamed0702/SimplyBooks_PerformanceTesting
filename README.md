# Performance Testing Summary Report
 
## Test Overview
The performance test was conducted on two APIs:
- **Booking API** (100 concurrent users)
- **Payment API** (200 concurrent users)
- **Total simulated users:** 300
 
---
 
## Key Metrics
 
| Metric | Booking API | Payment API | Total |
|--------|------------|------------|-------|
| # Samples | 100 | 200 | 300 |
| Average Response Time (ms) | 878 | 893 | 888 |
| Min Response Time (ms) | 801 | 773 | 773 |
| Max Response Time (ms) | 1153 | 1181 | 1181 |
| Standard Deviation | 92.65 | 95.31 | 94.68 |
| Error % | 0.00% | 0.50% | 0.33% |
| Throughput (Requests/sec) | 9.3/sec | 1.7/sec | 2.5/sec |
| Received KB/sec | 108.57 | 19.35 | 29.05 |
| Sent KB/sec | 2.56 | 0.46 | 0.69 |
| Avg. Bytes | 11,945.3 | 11,911.8 | 11,923.0 |
 
---
 
## Observations & Analysis
 
### **Booking API Performance**
- Average response time is **878ms**, which is within acceptable limits.
- No errors (**0.00%**), indicating stability.
- High throughput (**9.3/sec**) shows efficient handling of concurrent requests.
 
### **Payment API Performance**
- Average response time is **893ms**, slightly higher than Booking API.
- Error rate of **0.50%** suggests minor failures, but within an acceptable range.
- Lower throughput (**1.7/sec**) may indicate a bottleneck under load.
 
### **Overall System Performance**
- The total system maintained an **average response time of 888ms** across 300 users.
- Error rate remained low at **0.33%**.
- Booking API handled **higher throughput** compared to Payment API.
 
---
 
##  Recommendations
Optimize Payment API to handle concurrent users more efficiently and reduce errors.
Analyze throughput in Payment API for potential resource allocation issues.
Increase server scaling if higher concurrent users are expected in real-world scenarios.
Monitor database queries to optimize performance under load.
 
---
 
## Conclusion
The system performed well overall, with the **Booking API** handling requests efficiently. The **Payment API** showed minor errors and lower throughput, indicating areas for improvement. Further tuning and optimization are recommended to enhance performance.
