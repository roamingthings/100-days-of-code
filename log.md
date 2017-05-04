# 100 Days Of Code - Log

### Day 1: April 9, 2017

**Today's Progress**: Set up project modules for service and system test and implemented smoke test.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/85097afe3afe79a3fd1593d3a4d4c518f0d94f4e)

### Day 2: April 10, 2017

**Today's Progress**: Added a first entity (`RecurringExpense`) which is the core entity of the domain.

**Things I've learned**: I've started to big and wanted to put too much attributes and functionality into the first version. So I spend too much time thinking about details I might eventually need.  

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/1852d341011a5485016cbf6498d6195c4646e7d8)

**Resources**:
* [Agile Principle 5: Develop small, incremental releases and iterate](http://www.allaboutagile.com/agile-principle-5-how-do-you-eat-an-elephant/)

### Day 3: April 11, 2017

**Today's Progress**: Rewrote system test from yesterday as an integration test to discover the difference when using Tools provided by the Spring Framework. I'm not embracing it completely on purpose (yet). Will do more comparision and experimentation when the project becomes more complex.

**Things I've learned**: It's always gets hard when you start "fighting the system" by not using the tools provided but to force the framework into patterns you've learned with other frameworks. Figuring these things out also takes a lot of time.

**Things I've planned for tomorrow**: Add some more (complex) attributes and prepare a web ui.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/f28374c9d3d071a454cd85034ca8ab3dba94eeb3)

### Day 4: April 12, 2017

**Today's Progress**: Added entity listeners to update meta information regarding create and modify.

**Things I've learned**: Test support provided by the Spring Framework speeds up development of tests.

**Things I've planned for tomorrow**: Since I didn't get to this task today: Add some more (complex) attributes and prepare a web ui.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/ad98a329ed14509111d753c960c07d7698394d0f)

### Day 5: April 13, 2017

**Today's Progress**: Added infrastructure for UI using MVC and Thymeleaf.

**Things I've learned**: I'm used to implement views using JSF. I just learned that Thymeleaf behaves completely different.

**Things I've planned for tomorrow**: Improve the ui and feed in first "real" data.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/6572e51fe17e3f57e12ea9734a0c195f651e20e9)

### Day 6: April 14, 2017

**Today's Progress**: Pull UI into a separate project.

**Things I've learned**: I came to the conclusion that a separate UI project will introduce a clean separation between UI and service. I've been thinking if this is the right time to do this kind of split/refactoring or if it is better to continue implementing both parts in one project and do the refactoring later. However since I want to learn some best practices I decided to do the separation now.

**Things I've planned for tomorrow**: Again ;) Improve the ui and feed in first "real" data.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/7aa8ed1fe90d2c0b3de8829afe8c3b1f24246ef3)

### Day 7: April 15, 2017

**Today's Progress**: Moved to a new layout based on Bootstrap dashboard example and added a page example for editing.

**Things I've learned**: I've been used to write UIs using JSF. The more I get into Thymleaf I notice that the paradigm and mechanisms are completely different and I need some more time to wrap my head around. However I like the approach to first model in "pure" HTML and later switch to a Thymleaf template

**Things I've planned for tomorrow**: Use Thymeleaf to reuse parts of the UI.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/872a5fa414589f5ab3aa542e755b88ec77166567)

### Day 8: April 16, 2017 (Happy Easter)

**Today's Progress**: Figured out how to use the Thymeleaf layout mechanism. Added Font Awesome.

**Things I've learned**: Following an example that was using the Thymeleaf mechanism I almost freaked out since I couldn't get it to work in my project until I learned that and how I have to switch to Version 3 of Thymeleaf in my Spring Boot project.

**Things I've planned for tomorrow**: Utilize Thymeleaf to replace more static data with real values.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/43199acee6625180ad1ccb6fa4c7cb70b27d480e)

### Day 9: April 17, 2017 (Happy Easter)

**Today's Progress**: Learned about how to handle HATEOAS in the Spring Framework by getting a list of recurring expenses.

**Things I've learned**: HATEOAS is an interesting mechanism but hard to handle. The whole project starts to smell like Cargo Cult. I may start over with a much smaller / simpler approach.

**Things I've planned for tomorrow**: Try to extract the id from HATEOAS objects and decide to continue on this route or switch over to a monolith architecture (very likely).

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/88af7c7bf85d581169e5e0219ac50e43bb1653d6)

### Day 10: April 18, 2017

**Today's Progress**: Learned about projections when it comes to REST resources in Spring. List of expenses now contains "real" values.

**Things I've learned**: How to access the system id without parsing the link / resource that is included. I'm using a projection to add the entity id as a property `systemId` and use this in the list.

**Things I've planned for tomorrow**: Try to get the edit page working.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/4988fb7b4e3a0a0a1abdb7a7dfc3a7f96f1e4d31)

### Day 11: April 19, 2017

**Today's Progress**: Edit existing entities in a HTML form with Thymeleaf.

**Things I've learned**: I learned about the basic round trip, how Thymeleaf and Spring handle and convert data passed back and forth.

**Things I've planned for tomorrow**: Strengthen the form, Add validation (messages), create new instances and look for/compare with "best practices". _Most of all add tests!_

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/6be94ce653e2f229debbbe0de383c43cdaaf8e57)

### Day 12: April 20, 2017

**Today's Progress**: Added form validation.

**Things I've learned**: I learned about the basic validation mechanism in Spring MVC.

**Things I've planned for tomorrow**: Strengthen the form, Add validation (messages), create new instances and look for/compare with "best practices". _Most of all add tests!_

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/82ee5ba0139640d93a9c4214519cf7362c97d194)

### Day 13: April 21, 2017

**Today's Progress**: Added messages resource.

**Things I've learned**: I learned more about the validation and resource mechanism in Spring/Thymeleaf.

**Things I've planned for tomorrow**: Create new entities and look for/compare with "best practices". _Most of all add tests!_

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/a9d7daf2c43618962fecee1ebc05034cb10f3a64)

### Day 14: April 22, 2017

**Today's Progress**: Migrated to Thymeleaf layout dialect.

**Things I've learned**: I learned more about the layout method of Thymeleaf.

**Things I've planned for tomorrow**: Create new entities and look for/compare with "best practices". _Most of all add tests!_

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/a4300797da0b8916de98a8e414c68c4d8c6fb553)

### Day 15: April 23, 2017

**Today's Progress**: Wrote first MVC integration tests. Started migration to `LocalDate`.

**Things I've learned**: Learned about testing ov Spring MVC controllers including mocking. Also learned about using `LocalDate` instead of `Date`.

**Things I've planned for tomorrow**: Create new entities. Write more MVC integration tests.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/1b16be4ffb96891da700f45669f96d806b10abe8)

### Day 16: April 24, 2017

**Today's Progress**: Added a lot of Docker stuff: Building an image,orchestration with docker swarm and load balancing. Also new entities can now be created.

**Things I've learned**: Learned about building a docker image with gradle, pushing to a registry and setting up a container infrastructure with load balancing.

**Things I've planned for tomorrow**: Improve database setup and initialization.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/74530c34682aca4efaf582d0be50b995608e7ded)

### Day 17: April 25, 2017

**Today's Progress**: Added field reference number and started investigation about useful integration tests for MVC controller. Also made test profile configurable and only loading sample data in dev profile.

**Things I've learned**: Handling active profile for testing and developing stage.

**Things I've planned for tomorrow**: Get more into testing of an MVC controller.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/f380293215370774cf7ef71793b14cf50cb218d9)

### Day 18: April 26, 2017

**Today's Progress**: Added deletion of entities.

**Things I've learned**: Learned about how to delete using MVC.

**Things I've planned for tomorrow**: Change deletion to AJAX.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/384c22e4e9227bad8ed540c54a3393bfc7b4e287)

### Day 19: April 27, 2017

**Today's Progress**: Added deletion of entities by AJAX requests.

**Things I've learned**: Learned about how to partially render view in MVC and use AJAX.

**Things I've planned for tomorrow**: Look more into AJAX and partial view rendering.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/f359e4bda0bcce351545ae9ea4697756eef9c79a)

### Day 20: April 28, 2017

**Today's Progress**: Only a small update today. Cleaned up the script and added the list of last expenses to the home page.

**Things I've learned**: Externalizing the scripts and reuse fragments.

**Things I've planned for tomorrow**: Add security.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/fc7acee610b700f76a903d2d715e57fab4d904df)

### Day 21: April 29, 2017

**Today's Progress**: Started integrating security by implementing a simple sign in form.

**Things I've learned**: Spring security basics.

**Things I've planned for tomorrow**: Improve usage of Spring Security.

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/a353432c0729371adb3d11cc17ed6278ccad1ef6)

### Day 22: April 30, 2017

**Today's Progress**: Did a bit more security. Now logout is possible and user name is displayed.

**Things I've learned**: More on Spring Security.

**Things I've planned for tomorrow**:

**Link(s) to work**: [Expenses Service](https://github.com/roamingthings/expenses-service/commit/8522c5a78ee895d8eb585d84757e5791047856ef)

### Day 23: May 1, 2017

**Today's Progress**: Pulled persistence supporting classes into a separate project.

**Things I've learned**: A lot of gradle.

**Things I've planned for tomorrow**:

**Link(s) to work**: [Persistence Support](https://github.com/roamingthings/persistence-support/commit/7f02cc53c4c51a8e9c3035599c40bcc8d6996475)

### Day 24: May 2, 2017

**Today's Progress**: Added GitHub and facebook authorization using OAuth2.

**Things I've learned**: OAuth2 in Spring.

**Things I've planned for tomorrow**: Try to add local user accounts.

**Link(s) to work**: [Persistence Support](https://github.com/roamingthings/persistence-support/commit/7bd7869a1a10e8f27be1e8463b7c7fadce67afd8)

### Day 25: May 3, 2017

**Today's Progress**: Added handling of OAuth2 login result and introduced UserProfile.

**Things I've learned**: More OAuth2 in Spring.

**Things I've planned for tomorrow**: Continue on `UserProfile` handling/creation.

**Link(s) to work**: [Persistence Support](https://github.com/roamingthings/persistence-support/commit/87fd4361de9b8e2715448d8c1457f9ae467cd1ea)

### Day 26: May 4, 2017

**Today's Progress**: Still (unsuccesfully) trying to figure out how to create a local profile for a successful OAuth2 authentication.

**Things I've learned**: More Spring Security.

**Things I've planned for tomorrow**: Continue on `UserProfile` handling/creation.

**Link(s) to work**: [Persistence Support](https://github.com/roamingthings/persistence-support/commit/1f52f69e5782f99fe8289fcd30534714dc670069)
