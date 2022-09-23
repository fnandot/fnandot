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

## My principles

- 🧑‍💻 Write the code for your colleagues, not for machines.
- 🛠️ Pick the right tool for the right job, don't reinvent the wheel.
- 🤷‍♀️ Don’t solve a problem that doesn’t exist.
- 🫂 Listen. Inspire. Learn. Share.
- 🚀 Don’t walk alone, the mankind didn't get to the moon by only one person.
- 🥑 Be pragmatic, solve it and then iterate.

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
        Company("OLX Autos"),
        LocalDate.of(2022, 7, 1),
        LocalDate.now(),
        "Backend Chapter Lead",
        """
        As a backend chapter lead my role here is to play as an orchestrator to align efforts 
        between different squads. As well as a technical reference and cross-team mentor.
        Part of this role is to help building a backend community and promote knowledge sharing 
        across all devs, RFCs proposals, etc.
        """.trimIndent()
    ),
    Job(
        Company("OLX Autos"),
        LocalDate.of(2022, 1, 1),
        LocalDate.now(),
        "Senior Remote Software Engineer",
        """
        OLX lists around 500k cars on its platform every month and treated more than 
        50k inspections with a quotation for sale. In 2021 OLX Autos sold around 100k cars 
        and have more than 4,600 employees in the three continents and 10 markets 
        in which it operates.My role as a backend engineer is to help OLX continue to grow 
        and consolidate in LATAM and the rest of the markets.
        Among the technologies I work with here are Java/Kotlin with Spring Boot, 
        Infrastructure as Code with AWS and Terraform, pipeline definition with Gitlab CI/CD 
        and Kubernetes.
        """.trimIndent()
    ),
    Job(
        Company("Letgo"),
        LocalDate.of(2018, 1, 1),
        LocalDate.now(),
        "Senior Software Engineer",
        """
        When I joined Letgo in 2018 it was, with over 100M downloads and more than 20M 
        of monthly users, one the top downloaded second-hand marketplace Apps in USA. 
        The company was only 3 years old at 
        that moment and was growing fast, time-to-market was the priority and delivering 
        new features, always A/B tested, was our day to day.
        Among other things, working and dealing with high availability and large scale systems. 
        And how important is to have the correct logging and monitoring of your systems, 
        with approximately 700k daily users.
        Also designing solutions with different AWS (such DynamoDB, SQS, SNS, Aurora, etc) 
        """.trimIndent()
    ),
    Job(
        Company("La Salle BCN"),
        LocalDate.of(2020, 2, 1),
        LocalDate.of(2022, 1, 1),
        "Teacher",
        """
        As part of the faculty of the university master's degree 
        in high performance web programming at La Salle (Ramon Llull University, Barcelona). 
        My subject was development frameworks. 
        The course covers various topics to master modern backend frameworks such as 
        dependency injection containers, logging, ORM and data mapper patterns.
        """.trimIndent()
    ),
    Job(
        Company("Atrapalo"),
        LocalDate.of(2015, 11, 1),
        LocalDate.of(2018, 1, 1),
        "Senior Software Engineer",
        """
        When I joined Letgo in 2018 it was, with over 100M 
        downloads and more than 20M of monthly users, 
        one the top downloaded second-hand marketplace Apps in USA. 
        The company was only 3 years old at that moment and was 
        growing fast, time-to-market was the priority and delivering 
        new features, always A/B tested, was our day to day.
        Among other things, working and dealing with high availability 
        and large scale systems, by implementing microservices and 
        Event-Driven Architecture. Keeping in mind how important is 
        to have the correct logging and monitoring of your systems, 
        with approximately 700k daily users.
        Also designing solutions with different Amazon Web Services 
        (such DynamoDB, SQS, SNS, Aurora, etc).
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
	- Backend Chapter Lead at OLX Autos for 2 months
	- Senior Remote Software Engineer at OLX Autos for 8 months
	- Senior Software Engineer at Letgo for 4 years
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
