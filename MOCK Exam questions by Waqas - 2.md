# MOCK Exam questions by Waqas (part 2)

---

## Question 4

**a)** Explain the difference between the GPL license and the MIT license.

**b)** What does "share-alike" (copyleft) mean?

**c)** Give one GIS project that uses GPL and one that uses MIT.

### Answer

**a)** Both are open source licenses. The MIT license is very permissive: I can do almost anything with the code, even use it in closed source software, I just have to keep the attribution. The GPL is stricter: if I change the code and distribute it, my version also has to be released under the GPL.

**b)** Share-alike (copyleft) means that if I use or change the software, I must share my result under the same license. That way the software stays open.

**c)** GRASS GIS is GPL licensed (since 1999). UMN MapServer is MIT licensed (since 1999).

---

## Question 5

**a)** What is OGC and what does it do?

**b)** What is the OGC API?

**c)** What is meant by "Deprecation of OWS"?

### Answer

**a)** OGC is the Open Geospatial Consortium. It develops open standards for geospatial data and services, so that different software can work together.

**b)** OGC API is the newer family of OGC standards for web services (for example OGC API - Features for vector data). They are made for modern web development and are simpler to use than the old standards.

**c)** OWS means OGC Web Services, the older standards like WMS and WFS. "Deprecation" means they are still there and still work, but they are marked as outdated and OGC does not recommend them for new projects anymore. The idea is that the OGC API standards will replace them in the future.

---

## Question 6

**a)** What is the difference between git and GitHub?

**b)** What is the difference between a central and a distributed version control system?

**c)** If I do not have write access to a project on GitHub, how can I submit my changes?

### Answer

**a)** git is the version control software that runs on my computer. GitHub is a website (a server platform) where I can store git repositories and work together with others. GitHub is commercial and not open source. There are also other servers, like GitLab, Gitea or Forgejo.

**b)** In a central system the whole history is only on the server, and my computer has only one version of the files. In a distributed system (like git) every user has the whole history on their own computer, so I can work offline and no central server is needed (but usually there is one).

**c)** With a pull request:
1. Fork the repository on GitHub.
2. Clone my fork to my local computer (`git clone`).
3. Create a new branch (`git branch`, `git checkout`) and make my changes.
4. Stage and commit (`git add`, `git commit`).
5. Push to my fork on GitHub (`git push`).
6. Create a pull request on the GitHub website, so the owner of the original project can accept my changes.
