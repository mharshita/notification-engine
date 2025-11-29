# Notification Engine

Notification Engine in Java that simulates how real services send notifications (OTP, email alerts, promotional messages, etc.).
Instead of integrating with real SMS or email services, the engine will print logs to show that notifications are being sent.

Your system must support:

__1. Multiple Notification Types__

- OTP (highest priority, should be sent fastest)

- Transactional alerts

- Promotional messages (lowest priority)

__2. Priority Handling__

- Notifications must be processed in priority order, not just the order they are received.

__3. Parallel Processing__

- Multiple notifications should be processed in parallel using threads.

- OTPs should ideally be picked first and processed faster.

__4. Error Handling__

- Each notification should be processed inside try–catch.

- Failing tasks should not crash the engine.

__5. Logs__

- Every step should log what the system is doing.

- Example: “Queued OTP”, “Sending Email”, “Retrying”, “Completed”, etc.

### Goal

Build a modular, extensible notification engine with clean Java LLD, using OOP + interfaces + strategy-like patterns + thread management + queues.
