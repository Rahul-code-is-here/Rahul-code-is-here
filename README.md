<div align="center">

<!-- HERO TYPING SVG -->
<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=30&duration=3000&pause=1000&color=F74C00&center=true&vCenter=true&multiline=true&random=false&width=700&height=100&lines=%F0%9F%A6%80+Rahul+Chauhan;Rust+Backend+Engineer+%7C+Systems+Thinker" alt="Typing SVG" /></a>

<!-- PROFILE BADGES -->
<br/>

![Profile Views](https://komarev.com/ghpvc/?username=Rahul-code-is-here&color=F74C00&style=flat-square&label=PROFILE+VIEWS)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/-Rahul_Chauhan-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahul-chauhan-508968252/)
&nbsp;
[![Gmail](https://img.shields.io/badge/-rc9593912-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rc9593912@gmail.com)
&nbsp;
[![LeetCode](https://img.shields.io/badge/-rahultrambak89-FFA116?style=flat-square&logo=leetcode&logoColor=black)](https://leetcode.com/u/Rahul_LeetMaster/)

</div>

---

<!-- ABOUT BLOCK AS RUST STRUCT -->
```rust
pub struct RahulChauhan {
    role:       &'static str,  // "Rust Backend Developer @ TatvaSoft"
    location:   &'static str,  // "Bhavnagar, Gujarat, India"
    education:  &'static str,  // "B.E. IT | GEC Bhavnagar | 8.21 CGPA"
    currently:  &'static str,  // "Migrating Node.js backends to Rust"
    superpower: &'static str,  // "Turning runtime panics into compile-time errors"
}

impl RahulChauhan {
    pub const fn philosophy() -> &'static str {
        "If it compiles, it better be correct. Zero unwrap() in production."
    }
}
```

---

<!-- LANGUAGE PROFICIENCY - Based on actual work experience -->
### Language Proficiency

```text
Rust          ████████████████████░░░░░   80 %   Daily driver. Axum, SeaORM, Tokio, async/await.
SQL           ████████████████░░░░░░░░░   64 %   PostgreSQL, stored procs, query optimization.
C#/.NET       ████████████░░░░░░░░░░░░░   48 %   .NET Core MVC, Entity Framework, Web API.
JavaScript    ████████░░░░░░░░░░░░░░░░░   32 %   Node.js (MERN), migrating away from it.
Java          ██████░░░░░░░░░░░░░░░░░░░   24 %   DSA, academic projects.
HTML/CSS      █████░░░░░░░░░░░░░░░░░░░░   20 %   Bootstrap, responsive UI.
Python        ████░░░░░░░░░░░░░░░░░░░░░   16 %   Scripting & automation.
Bash          ███░░░░░░░░░░░░░░░░░░░░░░   12 %   Deployment scripts, CI/CD.
```

---

### Tech Arsenal

<table>
<tr>
<td align="center" width="50%">

**Backend & Systems**

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=F74C00)
![Axum](https://img.shields.io/badge/Axum-000000?style=for-the-badge&logo=rust&logoColor=F74C00)
![SeaORM](https://img.shields.io/badge/SeaORM-000000?style=for-the-badge&logo=rust&logoColor=F74C00)
![Tokio](https://img.shields.io/badge/Tokio-000000?style=for-the-badge&logo=rust&logoColor=F74C00)
![.NET](https://img.shields.io/badge/.NET_Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)

</td>
<td align="center" width="50%">

**Database & Cloud**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)
![AWS SAM](https://img.shields.io/badge/AWS_SAM-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![API Gateway](https://img.shields.io/badge/API_Gateway-FF4F8B?style=for-the-badge&logo=amazonapigateway&logoColor=white)

</td>
</tr>
<tr>
<td align="center" width="50%">

**Security & Auth**

![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![AES-256](https://img.shields.io/badge/AES--256_CBC/GCM-2C2C2C?style=for-the-badge&logo=letsencrypt&logoColor=F74C00)

</td>
<td align="center" width="50%">

**DevOps & Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

</td>
</tr>
</table>

---

### Ownership & Borrowing Journey

```rust
// Where I started:
fn main() {
    let data = get_data();
    let result = process(data.clone());   // .clone() everywhere, fighting the borrow checker
    println!("{:?}", result.unwrap());    // unwrap() and pray
}

// Where I am now:
fn main() -> Result<(), AppError> {
    let data = get_data()?;
    let result = process(&data)?;         // Borrowing with intent. Zero clones needed.
    println!("{result:?}");               // Errors are values, not panics.
    Ok(())
}
```

---

### Error Handling Discipline

```rust
// My production error pattern :
#[derive(Debug, thiserror::Error)]
pub enum ApiError {
    #[error("Database error: {0}")]
    Database(#[from] sea_orm::DbErr),

    #[error("Auth failed: {0}")]
    Unauthorized(String),

    #[error("Encryption error: {0}")]
    Crypto(#[from] aes_gcm::Error),

    #[error("Not found: {entity} with id {id}")]
    NotFound { entity: &'static str, id: String },
}

// Every error is typed. Every path is handled. No unwrap() in sight.
```

---

### What I Build

<table>
<tr>
<td width="50%">

**Production APIs in Rust**
- REST APIs with Axum + async/await
- Clean architecture (Controller / Service / Repository)
- OCPI 2.1.1 & 2.3 compliant APIs
- Custom auth middleware & token extractors

</td>
<td width="50%">

**Infrastructure & Security**
- AES-256-CBC/GCM encryption with proper IV handling
- AWS Lambda deployments via SAM
- API Gateway + Lambda Authorizers
- Centralized logging & request tracking middleware

</td>
</tr>
<tr>
<td width="50%">

**Database Engineering**
- PostgreSQL schema design with SeaORM
- Entity modeling & query optimization
- Stored procedures & database functions
- Migration management

</td>
<td width="50%">

**Migration Projects**
- Node.js (MERN) to Rust migration
- Performance analysis & optimization
- Async performance tuning
- Code reviews & refactoring

</td>
</tr>
</table>

---

### Featured Projects

| Project | What It Does | Stack |
|:--------|:-------------|:------|
| **Restaurant Management System** | Full-stack pizza shop system with CRUD, JWT auth, role-based access, stored procedures | `.NET Core MVC` `C#` `Entity Framework` `PostgreSQL` |
| **OCPI Backend APIs** | OCPI-compliant Location & Session modules for EV charging infrastructure | `Rust` `Axum` `SeaORM` `PostgreSQL` |
| **Crypto Service Module** | AES-256-CBC/GCM encryption service with key management and IV handling | `Rust` `aes-gcm` `AES-256` |
| **Auth Middleware** | Custom token-based authentication with extractors and Lambda authorizers | `Rust` `Axum` `AWS Lambda` `JWT` |

---

### Engineering Principles

```text
 Ownership > Garbage       Memory safety through the type system, not a runtime GC.
 Result<T,E> > panic!()    Every failure path is explicit and handled.
 &borrow > .clone()        If you're cloning, you haven't understood the data flow yet.
 Modules > Monoliths       lib.rs / main.rs separation. Every module earns its place.
 Compile-time > Runtime    Catch bugs before they ship. Trust the borrow checker.
```

---

### Currently Leveling Up

- **Async Rust Deep Dive** -- Pinning, `Future` trait internals, executor design
- **Advanced Lifetimes** -- Elision rules, borrow checker internals, self-referential structs
- **Systems Design** -- Distributed systems, consensus protocols, high-throughput pipelines
- **Open Source** -- Contributing to Rust ecosystem crates

---

<!-- GITHUB STATS -->
<div align="center">

### GitHub Stats

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Rahul-code-is-here&show_icons=true&hide_border=true&bg_color=0d1117&title_color=F74C00&icon_color=F74C00&text_color=c9d1d9&ring_color=F74C00&count_private=true&include_all_commits=true" alt="GitHub Stats" />
&nbsp;&nbsp;
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rahul-code-is-here&layout=compact&hide_border=true&bg_color=0d1117&title_color=F74C00&text_color=c9d1d9&langs_count=8" alt="Top Languages" />

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Rahul-code-is-here&hide_border=true&background=0d1117&stroke=30363d&ring=F74C00&fire=F74C00&currStreakLabel=F74C00&sideLabels=c9d1d9&currStreakNum=e6edf3&sideNums=e6edf3&dates=8b949e" alt="GitHub Streak" />

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Rahul-code-is-here&bg_color=0d1117&color=c9d1d9&line=F74C00&point=F74C00&area=true&area_color=F74C00&hide_border=true" alt="Contribution Graph" />

</div>

---

<!-- SNAKE ANIMATION -->
<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Rahul-code-is-here/Rahul-code-is-here/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Rahul-code-is-here/Rahul-code-is-here/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/Rahul-code-is-here/Rahul-code-is-here/output/github-snake-dark.svg" />
</picture>
</div>

---


<div align="center">

### Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahul-chauhan-508968252/)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rc9593912@gmail.com)

<br/>

## 🧮 LeetCode Profile

[![LeetCode](https://leetcard.jacoblin.cool/Rahul_LeetMaster?theme=dark)](https://leetcode.com/u/Rahul_LeetMaster/)

> 📈 I use LeetCode to sharpen problem-solving patterns and algorithmic thinking alongside my backend engineering work.


```rust
// Life is too short for garbage-collected languages.
// Let the compiler be your code reviewer.
```

<img src="https://capsule-render.vercel.app/api?type=waving&color=F74C00&height=80&section=footer" width="100%" />

</div>
