# MOCK Exam questions by Waqas

---

## Question 1

**a)** What is the difference between "free" as in freedom and "free of charge"?

**b)** What are the four freedoms of free software?

### Answer

**a)** "Free of charge" only means that I do not have to pay for the software. "Free" in free software means freedom: I am allowed to do things with the software. Free software can be sold, and software that costs nothing is not automatically free software.

**b)** The four freedoms:

1. Freedom to run the program for any purpose.
2. Freedom to study how the program works and change it to my needs.
3. Freedom to redistribute copies, so I can help my neighbour.
4. Freedom to improve the program and release my improvements to the public, so the whole community benefits.

---

## Question 2

**a)** What is open source software?

**b)** Google Maps is free to use. Is it open source? Explain.

### Answer

**a)** Open source software is software where the source code is public. Everybody can read it, use it, change it and share it, under the rules of its license (for example GPL or MIT).

**b)** No. Google Maps is free of charge for normal users, but it is not open source. I cannot see or change the source code, and I have to accept the EULA (terms of use), which restricts what I can do with the service and the data. So it is "free to use", but not "free" in the sense of freedom.

---

## Question 3

**a)** Name one of the oldest open source GIS software.

**b)** Tell what you know about its history.

### Answer

**a)** GRASS GIS.

**b)**
- It started in 1982 as a "Raster GIS", developed by the U.S. Army Corps of Engineers, Construction Engineering Research Laboratory (CERL).
- In the mid 1990s it was transferred to the "Open GRASS Consortium".
- In 1999 it was released under the GPL license.
- It is the oldest open source GIS and has about 40 years of development.

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
