## Architecture Overviev

**High Level Design:**
This is project particularly follows modular monolith architecture practices. The individual modules are loosely coupled for potential of this project breaking down into microservices down the line.
 ![alt text](https://github.com/tsartrooper/AuctionApplicationModularMonolith/blob/main/images/auction_application_hld.png)
Authentication(Spring Auth)
JWT based authentication Spring Auth was used. JWT was used instead of session/cookie based authentication to reduce the load on the server.

**Caching(Redis):**
For Caching, a key-value datastore, Redis a was used, because it has simple structure compared to other caches. 

**Scheduling(Spring Quartz Scheduler):**
For Scheduling Spring Quartz scheduler was used.

**Data Storage(Postgres):**
For Database Postgres was used.Port-Adapter Design pattern is implemented, to maintain interdependency between modules as loosely coupled as possible, this typically was inspired by modular monolilth architecture.

## Todo's
- [x] Authentication via google
- [x] Bids History
- [ ] Auctions Catalog Filter
- [ ] Profile
- [ ] Payment
- [ ] Push Notifications  

