## Hi there, my name is Nick 👋

Nice to meet you! You can read here about my journey and my experience over the past years

Once I finished managing a team up to 33 people from 7 cities I have decided to go back to technical problems and their solutions. 
I love to snowboard fast 🚀 and this love is spread on the Software. This is where my next stop have been: either it is a query to the database, website's content size, just an incorrect data structure used or gather&analyze of the statistics. 
I made [bitmap-usage](https://github.com/marniks7/bitmap-usage) service in `Go` with a problem close to real, and solution (bitmaps) to achieve low timings (measured in nanoseconds), and low memory footprint. Includes performance tests and measurement infrastructure.

---

After the performance activities my focus returned back to the development, and it was already the era of (micro)-services, `Spring Boot`, `Kubernetes`, `Cloud`, etc. My first tutor here is Chris Richardson's book `Microservices Patterns`. In the next few years I developed a set of libraries for Spring to cover logging, tracing, context propagation, etc. I developed many features in different services, like transactional counters, batch operations, efficient content streaming. At least one service developed by me from the scratch.

---

When I was working on the "performance", in that category were "all complex technical problems related to the resiliency", and in this new era it has become even more challenging. 
Did you face an issue on internal env - the service started to behave incorrectly? Usually reboot of the proper service will fix the issue, and if it does, the person may not raise the defect, even if it raises - there might not be enough information to analyze, and by the time the defect will be taken into assessment there will be no information on the env, e.g. because of the cleanup.

Let's talk about what is the problem here?
- Raising the defect and supporting it later requires effort.
- The person just needs a working environment to continue his actual work and raising the defect might look like extra.
- The person may not have enough expertise to effectively analyze&gather the info
- Imagine if after raising the defect if you will be asked for the test case (which you don't know and cannot reproduce).
- It often happens that the person who assesses the defect is not aware of the ways of solving such issues (without knowing the test case), as result defect might not be resolved at all.

What do I do? I prefer to make a fast assessment of the problem right away so that the nature of the problem is more or less clear and later work on the raised defect in a regular process.
Why do I talk about that? Sphere of my interests includes reasoning - it helps to see the problem and find a solution. And looks like I was just in the mood to talk about this topic ☺️
There is another solution, that can partially help here: dedicated `Chaos Engineering` team/activity. 
It was a great opportunity for me to explore complex cases, help other developers, and add a stability to the system in case of failures, like reboots, graceful shutdown, HA modes.
New infrastructure deployed from the scratch - `Kubernetes` with `ChaosMesh` and `Tekton` to manage pipelines. I developed all the parts needed for that integration, e.g. docker images with the tooling, queuing (kubernetes-controller) and pipelines with the test cases.
Obviously, most of the developed code is private, but there were 2 major open-source features (both merged) I made at home for Chaos Engineering activity - adding `YAML` editor to the pipelines [yaml editor UI PR](https://github.com/tektoncd/dashboard/pull/2575/) and feature [button to edit and run PR](https://github.com/tektoncd/dashboard/pull/2633). p.s. it was the first time I used `react` framework.

---

My own initiative included development of the `bash` scripts around Kubernetes for myself and teammates to speedup assessment of the defects, like gathering info from the pod: config variables, heapdumps, gc, logs, versions, etc.

---
I was responsible for the development of the `Quarkus` reactive application to solve the business need of the synchronization between two systems, including handling of large jsons, inter-component http communication and complex business logic.
And my projects at home included [UI-tool for mobile game](https://github.com/marniks7/nmd-arena-source) with the first time usage of `Vue` framework.

---

And my current project is a development of the proxy to replace system A to B without changes on the client side. I take responsibility to make sure that the service will be `maintainable` over the years. I like to think that I share my knowledge about the features in the form of the `unit and integration tests` for future me or teammates and our `users` are not impacted when we are dealing with the changes.

---
Summary:
In our development handicraft, I think about languages and services like the tools: use the most applicable one! 
Among my languages are `Java`, `Go`, `JavaScript/TypeScript` and `Python`, messaging/streaming services (`RabbitMQ`, `Kafka`), and a databases (`Postgres`, `Oracle`), Cloud Services (`GKE`) and many other services, tools&utilities, frameworks.
My experience includes large enterprise solutions, small webapps and a little bit of open source: from 0 to Production and all the way after.
