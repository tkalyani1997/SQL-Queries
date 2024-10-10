# Troubleshoot slow-running queries in SQL Server

If your query is running slow, the first step is to check if it's **waiting** or **running**. 

💡 **Tip:** If CPU time is less than 70-80% of the total duration, you're likely dealing with a waiting issue. Focus on reducing wait times to improve efficiency!

👉 **Waiting Query (Low CPU Usage):**
- Lock waits
- Memory waits
- I/O waits (PAGEIOLATCH, WRITELOG)
- Network waits (ASYNC_NETWORK_IO)
- Latch waits (PAGELATCH)
- SOS Scheduler Yield waits
- Other Waits...

👉 **Running Query (High CPU Usage):**
- Long compilation times
- Long execution times
