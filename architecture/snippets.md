# Architecture

## SDLC

- Define the customer requirements for the solution
- Design a great solution to meet those requirements
- Implement the designed solution
- Validate the solution with your customer
- Deliver the solution in the working environment

## Fundamental Constraints

- The solution needs to meet user requirements
- The solution needs to be delivered on time
- The solution needs to adhere to the project budget
- The solution needs to deliver good quality
- The solution needs to guarantee safe and effective future evolution

## Lean Principles for Software Development

> Written by Mary and Tom Poppendieck

1. **Eliminate waste:** You may consider waste to be anything that will interfere with the delivery of the real need of the customer.
2. **Build quality in:** An organization that wants to guarantee quality needs to promote it in processes from the very beginning, instead of only considering it when code is being tested.
3. **Create knowledge:** All companies that have achieved excellence have a common pattern of generating new knowledge by disciplined experimentation, documenting that knowledge, and guaranteeing that it is spread all over the organization.
4. **Defer commitment:** Plan decisions at the latest possible moment without causing damage to the project.
5. **Deliver fast:** The faster you deliver software, the more elimination of waste you have. Companies that compete using time frequency have significant advantages over their competitors.
6. **Respect people:** Giving reasonable objectives to the team, together with plans that will guide them to self-organize their routine, is a matter of respecting the people that you work with.
7. **Optimize the whole:** A Lean company improves the cycle of value, from the moment it receives a new requirement to the point at which it delivers the software.

## Capturing NFR's

Non functional requirements are important to capture and know up front as they can affect the architecture.

- **Scalability:** As a software developer, globalization gives you the opportunity to have your solution running all over the world. This is fantastic, but you, as a software architect, need to design a solution that provides that possibility. Scalability is the possibility for an application to increase its processing power as soon as it is necessary, due to the number of resources that are being consumed.

- **Robustness:** No matter how scalable your application is, if it is not able to guarantee a stable and always-on solution, you are not going to get any peace. Robustness is important for critical solutions, where you do not have the opportunity for maintenance at any time due to the kind of problem that the application solves. In many industries, the software cannot stop, and lots of routines run when nobody is available (overnight, during holidays, and so on). Designing a robust solution will give you the freedom to live while your software is running well.

- **Security:** This is another really important area that needs to be discussed after the requirements stage. Everybody worries about security, and different laws dealing with it are in place in different parts of the world. You, as a software architect, must understand that security needs to be provided by design. This is the only way to cope with all the needs that the security community is discussing right now.
  
- **Performance:** The process of understanding the system you are going to develop will probably give you a good idea of what you will need to do to get the desired performance from the system. This topic needs to be discussed with the user, to identify most of the bottlenecks you will face during the development stage.

## Design Tecniques

### Googles Design Sprint

**Design Sprint** is a process focused on solving critical business questions through design in a five-day sprint. This technique was presented by Google, and it is something that allows you to quickly test and learn from an idea when you are looking to build and launch a solution to market.

The process involves experts spending a week to solve the problem at hand, in a war room prepared for that purpose. The week is like this:

- **Monday:** The focus of this day is to identify the target of the sprint and map the challenge to achieve it.

- **Tuesday:** After understanding the goal of the sprint, participants start sketching solutions that may solve it. It is time to find customers to test the new solution that will be provided.

- **Wednesday:** This is when the team needs to decide the solutions that have the greatest chance to solve the problem. The team must draw these solutions into a storyboard, preparing a plan for the prototype.

- **Thursday:** It is time to prototype the idea planned on the storyboard.

- **Friday:** Having completed the prototype, the team presents it to customers, learning by getting information from their reaction to the solution designed.