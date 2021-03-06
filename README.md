# N-Tier Architecture or Layered Architecure

The most common architecture pattern is the layered architecture pattern, otherwise known as the n-tier architecture pattern. This pattern is the de facto standard for most Java EE applications and therefore is widely known by most architects, designers, and developers. The layered architecture pattern closely matches the traditional IT communication and organizational structures found in most companies, making it a natural choice for most business application development efforts.

# Pattern Desription

Components within the layered architecture pattern are organized into horizontal layers, each layer performing a specific role within the application (e.g., presentation logic or business logic). Although the layered architecture pattern does not specify the number and types of layers that must exist in the pattern, most layered architectures consist of four standard layers: presentation, business, persistence, and database. In some cases, the business layer and persistence layer are combined into a single business layer, particularly when the persistence logic (e.g., SQL or HSQL) is embedded within the business layer components. Thus, smaller applications may have only three layers, whereas larger and more complex business applications may contain five or more layers.

One of the powerful features of the layered architecture pattern is the separation of concerns among components. Components within a specific layer deal only with logic that pertains to that layer. For example, components in the presentation layer deal only with presentation logic, whereas components residing in the business layer deal only with business logic. This type of component classification makes it easy to build effective roles and responsibility models into your architecture, and also makes it easy to develop, test, govern, and maintain applications using this architecture pattern due to well-defined component interfaces and limited component scope.

# Diagram

![](images/diagram.png)
![](images/diagram2.png)
# References

- Richards, M. (2015). Software architecture patterns (Vol. 4). 1005 Gravenstein Highway North, Sebastopol, CA 95472: O'Reilly Media, Incorporated.
- Martin, R. C., Grenning, J., & Brown, S. (2018). Clean architecture: a craftsman's guide to software structure and design (No. s 31, pp. 57-91). Prentice Hall.
- https://enqueuezero.com/layered-architecture.html
- https://medium.com/@alameerashraf/nodejs-a-clean-architecture-931898b00d68

# Folder Structure using Layerd Architecture

Separate concerns among components:

```
my-project/
????????? node_modules/
????????? config/
???   ????????? utils.js
????????? components/
????????? modules/
???   ???   ????????? profile/
???   ???   ???   ????????? routesProfile.js
???   ???   ???   ????????? serviceProfile.js
???   ???   ???   ????????? dalProfile.js
???   ???   ???   ????????? index.js
???   ???   ????????? ...
????????? pages/
???   ????????? profile.js
???   ????????? index.js
????????? public/
???   ????????? styles.css
????????? app.js
????????? routes.js
????????? package.json
????????? package-lock.json
????????? README.md
```
Package by Layer:

```
my-project/
????????? node_modules/
????????? api/
????????? aplication/
????????? common/
????????? infrastructure/
????????? loaders/
????????? models/
????????? services/
????????? server.js
????????? package.json
????????? package-lock.json
????????? README.md
```

# Generate Slides

To generete the slides just enter the following command in the project folder:

```sh
$ npx @marp-team/marp-cli@latest slides.md
```
> To see the slides just open the the `slides.html` file in the browser