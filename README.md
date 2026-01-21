#   Monolithic Architecture (FastAPI)

## Name:
Surabhi M  
## SRN:
PES1UG23AM325  

## Description
This project demonstrates a monolithic web application built using FastAPI for Cloud Computing Lab 2. All functionalities such as registration, login, events, my-events, and checkout are implemented in a single codebase and deployed as one unit.

The lab highlights the drawbacks of monolithic architecture by introducing an intentional crash in the checkout route, fixing the issue, and performing load testing using Locust. Performance optimization is then applied to improve response times.

---

## Screenshots

- SS1 – Events page loaded  
- SS2 – Checkout crash  
- SS3 – Checkout fixed  
- SS4 – Locust checkout load test  
- SS5 – Checkout after optimization  
- SS6 – Events before optimization  
- SS7 – Events after optimization  
- SS8 – My-events before optimization  
- SS9 – My-events after optimization  

---

## Optimizations

### Events Route

**Bottleneck:**  
The events route lacked proper response validation and clear performance tracking.

**Change Made:**  
Response validation and named requests were added in the Locust test.

**Why Performance Improved:**  
Accurate request tracking improved reliability of performance analysis.

---

### My-Events Route

**Bottleneck:**  
The my-events route did not validate responses, leading to inaccurate performance results.

**Change Made:**  
Response validation and request naming were added.

**Why Performance Improved:**  
Only successful responses were counted, improving measurement accuracy.

---

## Conclusion
This lab demonstrates how monolithic applications can fail due to a single module issue and how internal optimization and testing can improve performance and reliability.
