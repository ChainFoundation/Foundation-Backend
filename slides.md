---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

![bg left:40% 80%](images/layers.png)

# **N-Tier Architecture**
# **Layered Architecture🔥**

---

# Layared Architecture

![bg left 100%](images/layered-architecture-pattern.png)

The layered architecture pattern closely matches the traditional IT communication and organizational structures found in most companies, making it a natural choice for most business application development efforts.

---

# Key Concepts

![bg left 90%](images/key-concepts.png)

- Closed layer
- The layers of isolation

---

# Key Concepts

![bg left 90%](images/open-layer.png)

Leveraging the concept of open and closed layers helps define the relationship between architecture layers and request flows and also provides designers and developers with the necessary information to understand the various layer access restrictions within the architecture.

---

# Pros and Cons

- Advantages
  - Separate of concern
  - More testable
  - Isolation
  - Changeability
- Disdvantages
  - The performance is getting slower as more and more layers added.
  - Leaky abstraction can disturb your layered intent.

---

# Pattern Example

![bg left 100%](images/layered-example.png)

Request from a business user to retrieve customer information for a particular individual.

---

# NodeJS Project Folder structure