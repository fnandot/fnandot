# Fernando Pradas
![Website](https://img.shields.io/website?url=http%3A%2F%2Ffernandopradas.com)
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

+ 🧑‍🔬 Science Divulgation
+ 🤖 AI Artificial Intelligence
+ ⛓ Blockchain & Smart Contracts (Specially in Ethereum)
+ ✈ Travelling

## Experience
```kotlin
import java.time.LocalDate
import java.time.Period

@JvmInline
value class Company(val name: String)

data class Job(
    val company: Company,
    val startDate: LocalDate,
    val endDate: LocalDate,
    val title: String,
    val description: String
) {
    internal val period: Period = Period.between(startDate, endDate)
}

fun Job.toStringPeriod() = period
    .takeIf { it.years > 0 }?.let { "${it.years} years" } ?: "${period.months} months"

val professionalCareer = listOf(
    Job(
        Company("Letgo"),
        LocalDate.of(2018, 1, 1),
        LocalDate.now(),
        "Remote Senior Software Engineer",
        """
        When I joined Letgo in 2018 it was, with over 100M downloads and more than 20M of monthly users, 
        one the top downloaded second-hand marketplace Apps in USA. The company was only 3 years old at 
        that moment and was growing fast, time-to-market was the priority and delivering new features, 
        always A/B tested, was our day to day.
        Among other things, working and dealing with high availability and large scale systems. 
        And how important is to have the correct logging and monitoring of your systems, 
        with aproximately 700k daily users.
        Also designing solutions with different AWS (such DynamoDB, SQS, SNS, Aurora, etc) 
        """.trimIndent()
    ),
    Job(
        Company("La Salle BCN"),
        LocalDate.of(2020, 2, 1),
        LocalDate.of(2022, 1, 1),
        "Teacher",
        """
        As part of the faculty of the university master's degree in high performance web programming at 
        La Salle (Ramon Llull University, Barcelona), my subject is development frameworks. 
        The course covers various topics to master modern backend frameworks such as dependency injection containers, 
        logging, ORM and data mapper patterns.
        """.trimIndent()
    ),
    Job(
        Company("Atrapalo"),
        LocalDate.of(2015, 11, 1),
        LocalDate.of(2018, 1, 1),
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
        """.trimIndent()
    ),
    Job(
        Company("Bab"),
        LocalDate.of(2012, 12, 1),
        LocalDate.of(2015, 11, 1),
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
        """.trimIndent()
    )
)

fun main() = println(
    professionalCareer
        .sortedByDescending { it.endDate }
        .joinToString(System.lineSeparator()) { "\t- ${it.title} at ${it.company.name} for ${it.toStringPeriod()}" }
        .let { "Professional career:${System.lineSeparator()}$it" }
)
/*
Professional career:
	- Remote Senior Software Engineer at Letgo for 4 years
	- Teacher at La Salle BCN for 1 years
	- Senior Software Engineer at Atrapalo for 2 years
	- Full-stack Developer at Bab for 2 years
*/
```

## Languages
```javascript
let programmingLanguages = [
  "PHP",
  "Javascript",
  "Bash",
  "Go",
  "Scala",
  "Kotlin",
  "Solidity",
];

let spokenLanguages = [
  "Spanish",
  "Catalan",
  "English"
];

console.log(`I'm proficient in ${programmingLanguages.slice(0, -1).join(", ")} and ${programmingLanguages.slice(-1)}.`);
console.log(`I speak ${spokenLanguages.slice(0, -1).join(", ")} and ${spokenLanguages.slice(-1)}.`);

/*
I'm proficient in PHP, Javascript, Bash, Go, Scala, Kotlin and Solidity.
I speak Spanish, Catalan and English.
*/
```

## My philosophy

- `write code for humans and not for machines` is my main principle while I'm developing. 
- `be a team player` because to reach the moon it was not thanks to a single person, but the collaboration between thousands of people.
- ...
