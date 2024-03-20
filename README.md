# ProducerConsumer-with-Semaphores

This project implements a producer-consumer system in Java using semaphores for synchronization. The producer-consumer problem is a classic synchronization problem where multiple producer threads produce items, which are then consumed by multiple consumer threads. Semaphores are used to control access to a shared buffer to ensure that producers and consumers can work concurrently without conflicts.

Semaphores are used to control access to the shared buffer:
A semaphore is used to track the number of empty slots in the buffer. When a producer wants to produce an item, it waits until there is an empty slot available.
Another semaphore is used to track the number of filled slots in the buffer. When a consumer wants to consume an item, it waits until there is a filled slot available.
