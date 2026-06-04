# TradeFlow_prototype

link: https://aesthetic-torte-22ff74.netlify.app/  (Netlify Drop ver.)

a digital trade operations platform designed for managing international shipments and supply chain logistics. It combines AI-powered analytics, real-time GPS tracking, blockchain document verification, and supply chain finance into a single dashboard — similar to how Taobao integrates e-commerce operations.

## Functions - 6 Main Modules
### 1. 📊 Dashboard (仪表板)
The central hub showing a real-time overview of all operations:
Key stats: Active shipments, total trade value, pending documents, active alerts
Shipment table: Lists all cargo with route, status, value, temperature, and ETA
Document verification panel: Tracks legal documents (Bill of Lading, Invoices, Certificates) with status (Verified / Pending / Rejected)
Environmental monitoring: Live temperature, humidity, and location data for containers with a trend chart
Risk alerts: High/medium priority warnings (e.g., temperature threshold exceeded)
### 2. AI Analytics (AI 分析)
Machine learning predictions for delivery forecasting:
Model accuracy stats: 96.8% accuracy, 47 predictions today, 92.4% confidence
Prediction accuracy chart: Compares AI predictions vs actual outcomes per shipment
Delivery risk predictions: Each shipment rated Low / Medium / High risk with:
On-time probability (progress bar)
Predicted delay in hours
Risk factors (weather, customs, docs, congestion)
AI recommendation (e.g., "Monitor customs closely" or "Immediate reroute needed")
Run Prediction button: Triggers a fresh AI analysis
### 3. 🛰️ GPS Tracking (GPS 追踪)
IoT-enabled live vessel tracking with satellite integration:
Fleet stats: Active vessels, average speed, signal quality, last update time
Live map: Shows 3 ships (Pacific Star, Atlantic Wave, Ocean Explorer) with pulsing markers that move in real time
Real-time data updates every second: Speed (with 14 decimal precision), heading, position
Pause/Resume button: Stops the live feed
Click any ship → shows full details (IMO number, flag, vessel type, cargo, draft, destination, ETA)
### 4. ⛓️ Blockchain Verification (区块链)
Immutable document verification on a distributed ledger:
Network stats: Total blocks (847,392), verified docs (2,847), nodes (47), block time (2.1s)
Recent transactions: Each document's verification event with status (Verified on Chain / Mined / Pending Mining)
Click a block → shows block hash, timestamp, verifier nodes, confirmation status
Verify Document button: Opens a form to upload and verify new documents on-chain
### 5. ⚠️ ML Exception Handling (异常处理)
Automated anomaly detection and resolution:
Stats: Auto-resolved (342), active (4), avg resolution time (12 min), success rate (94.6%)
Exception list: Each item has severity (Critical / High / Medium / Low), description, ML confidence score
Auto-Resolve button: Simulates ML fixing the issue (spinner → resolved)
Manual Resolve: Opens a form for notes
Escalate: Sends to senior team
Scan Now: Triggers a new ML scan for anomalies
### 6. 💰 Supply Chain Finance (财务)
Payment and trade finance management:
Monthly revenue trend: Bar chart showing 6-month revenue
Payment status distribution: Doughnut chart (Paid 65% / Pending 25% / Overdue 10%)
Recent transactions table: ID, shipment, type (Letter of Credit / Wire Transfer / Invoice), counterparty, amount, status
New Transaction button: Form to create letters of credit, wire transfers, or invoices
Export: Download transactions as CSV
## Shared Features
- 🌐 Multilingual: Toggle between Simplified Chinese (default) and English — all UI text, charts, toasts, and modals translate instantly. Language persists via localStorage.
- 🔔 Notifications: Bell icon with badge count, dropdown showing recent alerts, "Mark all read"
- 👤 User Profile: Shows Operations Manager with logout/settings options
- 🔍 Global Search : Top search bar for quick access
- 🍞 Toast Messages: All actions trigger success/info/warning toasts
- 📋 Modals: Reusable modal system for details, forms, and confirmations
- 📱 Responsive: Adapts to desktop/tablet/mobile layouts
