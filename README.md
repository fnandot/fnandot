# Hello World
![Website](https://img.shields.io/website?url=http%3A%2F%2Fwww.fernandopradas.com)
![Build Passing](https://img.shields.io/badge/build-passing-brightgreen)
![Tests Passing](https://img.shields.io/badge/test-passing-brightgreen)
![Code Quality](https://img.shields.io/badge/code%20quality-A-brightgreen)
![Languages](https://img.shields.io/badge/languages-5-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![GitHub last commit](https://img.shields.io/github/last-commit/letnando/webpage)

[![GitHub followers](https://img.shields.io/github/followers/fnandot?style=social)](https://github.com/fnandot)
[![Twitter Follow](https://img.shields.io/twitter/follow/fnandot?style=social)](https://twitter.com/intent/follow?screen_name=fnandot)

## What I do?

I'm a software engineer with wide experience in development.

I've had the opportunity to participate in the development of exciting 🤩 projects that have helped me to learn 🤔 actively. When I develop software my main goal 🚩is to solve problems with a clean 🧽, reusable ♻️ and scalable ⬆️ code. I'm always looking for 🔎 how to improve myself and how to improve the code and its performance, this is really important 🔝 in large volume projects.

Adaptability and multidisciplinary teamwork 👥, and seeking always to keep abreast of new trends 🆕 in a world 🌎 of constant change, as is the development of software.

I recently started in the 🎓 teaching world as a Frameworks teacher at LaSalleBCN (URL University).

On my free time 🥳 I love to travel ✈️ and learning about science ⚛ divulgation. 

## Interests

+ Science Divulgation
+ AI Artificial Intelligence
+ Blockchain & Smart Contracts (Specially in Ethereum)
+ ...

## Experience
```scala
case class Company(val name: String);
case class Job(
  val company: Company, 
  val name: String, 
  val description: String
);

val professionalCareer = List(
  Job(
    Company("Letgo"),
    "Senior Backend Engineer",
    """
      When I joined Letgo in 2018 it was, with over 100M downloads and more than 20M of monthly users, one the top downloaded second-hand marketplace Apps in USA.       The company was only 3 years old at that moment and was growing fast, time-to-market was the priority and delivering new features, always A/B tested, was         our day to day.
      Among other things, working and dealing with high availability and large scale systems. And how important is to have the correct logging and monitoring of         your systems, with aproximately 700k daily users.
      Also designing solutions with different AWS (such DynamoDB, SQS, SNS, Aurora, etc) 
    """
  ),
  Job(
    Company("Atrapalo"),
    "Senior Software Engineer",
    """
      When I joined Atrápalo the company was in the path 
      of migrating from monolith to microservices. So my 
      work there was to keep working on that direction 
      by creating new microservices from the scratch, 
      always applying DDD.Maintain the legacy codebase 
      was also important and adapting it to the new 
      architecture. Also, during my Atrápalo journey 
      I learned a lot of DevOps culture 
      (mainly Docker, Jenkins Pipelines)
    """
  ),
  Job(
    Company("Bab"),
    "Full-stack Developer",
    """     
    A small company with 12-14 employees mainly focused 
    on and SaaS product consisting of a CMS + e-commerce, 
    but also developing custom projects for clients.
    My job here, mainly, was to participate in all phases 
    (requirements, design and development) of projects 
    from our clients. Projects such a MOOC platform or an 
    online magazine kiosk. Also helped in the first steps 
    of designing the new version of CMS platform.
    """
  )
);

val companies = professionalCareer
    .reverse
    .map(_.company.name)
    .reduce(_ + " => " + _);
    
print(s"Companies I've worked: ${companies}");
// Companies I've worked: Bab => Atrapalo => Letgo
```

## Languages
```javascript
let programmingLanguages = [
  "PHP",
  "Javascript",
  "Bash",
  "Go",
  "Scala"
];

let spokenLanguages = [
  "Spanish",
  "Catalan",
  "English"
];
```

## Philosophy

- `write code for humans and not for machines` is my main principle while I'm developing. 
- `be a team player` because to reach the moon it was not thanks to a single man, but the collaboration between thousands of people.
- ...
