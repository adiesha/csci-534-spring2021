# Computational Geometry: CSCI 534

**NOTE: This is a live document and is subject to change throughout the
semester.**

Spatial data is everywhere.  How do we organize that data so that it can be
efficiently processed?  Moreover, how can we extract meaning out of this data?
Computational Geometry provides tools for solving these questions.  In this
class, we will study convex hulls, Delauney triangulations, Voronoi diagrams,
graph drawing, meshing, spatial decompositions, and many other geometric
techniques.  In addition, we will have opportunities to apply the techniques to
real world problems.

The techniques of computational geometry are very useful!  Indeed, they are part
of the algorithmic foundations of Graphics, Visualization, Data Mining,
Databases, Sensor Networks, Machine Learning, and Geographic Information
Systems.  They are also integral to simulation techniques used by Engineering,
Computational Physics and Biology... just to name a few.

## Meeting Times

Tue, Thurs 12:15 - 13:30 [On Zoom](https://zoom.us/j/92140915457)

## Instructor

David L. Millman, Ph.D.

**Email**: david.millman@montana.edu

**Office hours**: Fri 15:00-17:00, or by [appointment](https://calendly.com/dmillman)

**Office**: [On Webex](https://bit.ly/webex-with-dave)

**Github**: [dlm](https://github.com/dlm)

## Textbooks

Required:

* [David Mount's lecture notes](http://www.cs.umd.edu/class/fall2014/cmsc754/Lects/cmsc754-fall14-lects.pdf) (DMLN in reading below)

Optional but recommended:

* [Computational Geometry: Algorithms and Applications](https://link.springer.com/book/10.1007%2F978-3-540-77974-2) by Mark de Berg, Otfried Cheong, Marc van Kreveld, Mark Overmars (CGAA in reading below).
* [Discrete and Computational Geometry](https://press.princeton.edu/titles/9489.html) by Satyan L. Devadoss and Joseph O'Rourke
* [Computational Geometry in C (Second Edition)](https://cs.smith.edu/~jorourke/books/compgeom.html) by Joseph O'Rourke
* [Graph Drawing](https://www.pearson.com/us/higher-education/program/Tollis-Graph-Drawing-Algorithms-for-the-Visualization-of-Graphs/PGM36916.html) by Giuseppe Di Battista, Peter Eades, Roberto Tamassia, Ioannis G. Tollis (GC in reading below).

## Class schedule

The lecture schedule is subject to change throughout the semester, but here is
the current plan. Assignments and due dates will be updated as they're assigned
in class.

### Jan

| Date | Description                                    | Assigned             | Due                  | Recommended Reading                        | Video                                                              |
|------|------------------------------------------------|----------------------|----------------------|--------------------------------------------|--------------------------------------------------------------------|
| 1/12 | [Intro](./notes/2021-01-12.pdf)                |                      |                      | DMLN L1, CGAA 1                            | [1](https://montana.box.com/s/vqdx6dkjakuwqkhzybxubqdmifgb4ysn)    |
| 1/14 | [Warm-up: Slope Stats](./notes/2021-01-14.pdf) |                      |                      | DMLN L2                                    | [1](https://montana.box.com/s/aqbkivfrilf8dsznh4ye4k8q3ad92qyv)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 1/19 | [Convex Hull](./notes/2021-01-19.pdf)          |                      |                      | DMLN L3, CGAA 1.1                          | [1](https://montana.box.com/s/17ljdso22a993lzzjfejgkydl0duzlll)    |
| 1/21 | [Convex Hull 2](./notes/2021-01-21.pdf)        | [HW 01](./hw/01.pdf) |                      | DMLN L4                                    | [1](https://montana.box.com/s/5btgqonj8vfl1eknu6c8j7gvvqz3dbqc)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 1/26 | [Seg Intersect](./notes/2021-01-26.pdf)        |                      |                      | DMLN L5, CGAA 2.1                          | [1](https://montana.box.com/s/twlsoy2xkmoejeaqypuegh9oxskt2kcw)    |
| 1/28 | [Seg Intersect 2](./notes/2021-01-28.pdf)      |                      | [HW 01](./hw/01.pdf) | DMLN L5, CGAA 2.1                          | [1](https://montana.box.com/s/eias1xo869v3icu56lhooe7h81gx3r9v)    |

### Feb

| Date | Description                                    | Assigned             | Due                  | Recommended Reading                        | Video                                                              |
|------|------------------------------------------------|----------------------|----------------------|--------------------------------------------|--------------------------------------------------------------------|
| 2/02 | [DCEL](./notes/2021-02-02.pdf)                 |                      |                      | DMLN L24, CGAA 2.2-.3                      | [1](https://montana.box.com/s/8zuz9fc84ckja73l6dxsxifrlb7lr6xq)    |
| 2/04 | [Polygon triangulation](./notes/2021-02-04.pdf)| [HW 02](./hw/02.pdf) |                      | DMLN L6, CGAA 3.2                          | [1](https://montana.box.com/s/se3imniq2jwhaixh39v4p2trvjq2qy4b)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 2/09 | [Poly Triang pt 2](./notes/2021-02-09.pdf)     |                      |                      | DMLN L6, CGAA 3.2                          | [1](https://montana.box.com/s/v7ylrg2mi63ki2xkxoyp1cv1gorwv8xy)    |
| 2/11 | [Polygon Guarding](./notes/2021-02-11.pdf)     |                      | [HW 02](./hw/02.pdf) | CGAA 3.1-.2                                | [1](https://montana.box.com/s/jiue1drr3valzb4bc30hyd3izkksxodr)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 2/16 | [GD: Rooted Trees](./notes/2021-02-16.pdf)     |                      |                      | GD 3                                       | [1](https://montana.box.com/s/xs8kiqm1gxuhkrukaekgsdsvulqb76no)    |
| 2/18 | Exam 1                                         |                      |                      |                                            |                                                                    |
|      |                                                |                      |                      |                                            |                                                                    |
| 2/23 | [Traps](./notes/2021-02-23.pdf)                |                      |                      | DMLN L9, GCAA 6.1-.2                       | [1](https://montana.box.com/s/eqit1unrpzf6ap8shm82f7pq3gqtk0wh)    |
| 2/25 | [Traps 2](./notes/2021-02-25.pdf)              |                      |                      | DMLN L9-10, CGAA 6.1-.2                    | [1](https://montana.box.com/s/fo51npkr1fjqib5o9gps1v4gbm52fufk)    |

### March

| Date | Description                                    | Assigned             | Due                  | Recommended Reading                        | Video                                                              |
|------|------------------------------------------------|----------------------|----------------------|--------------------------------------------|--------------------------------------------------------------------|
| 3/02 | [Traps 3](./notes/2021-03-02.pdf)              | [HW 03](./hw/03.pdf) |                      | DMLN L10, CGAA 6.1-.2                      | [1](https://montana.box.com/s/8rnntyjfn4havw1dxg37mffax6nx8phv)    |
| 3/04 | [1/2-Plane Intersect](./notes/2021-03-04.pdf)  |                      |                      | DMLN L7, CGAA 4.2                          | [1](https://montana.box.com/s/02z66tn6bw8rg2gocpovxkhtlpoxha7u)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 3/09 | [LP 1](./notes/2021-03-09.pdf)                 |                      | [HW 03](./hw/03.pdf) | DMLN L8, CGAA 4.3-.6                       | [1](https://montana.box.com/s/32oosmp4i7eafrfojojjmq7ou1dgvzn8)    |
| 3/11 | [LP 2](./notes/2021-03-11.pdf)                 | [HW 04](./hw/04.pdf) |                      | DMLN L8, CGAA 4.3-.6                       | [1](https://montana.box.com/s/ws77sns3lbg383jgl7u9e21s8i2g0xpv)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 3/16 | [Voronoi Diagram](./notes/2021-03-16.pdf)      |                      |                      | DMLN 11, CGAA 7.1-.2                       | [1](https://montana.box.com/s/vsay9lc7107go7d3ras1tdptz48jkbrh)    |
| 3/18 | [Fortunes Algo](./notes/2021-03-18.pdf)        | [HW 05](./hw/05.pdf) | [HW 04](./hw/04.pdf) | DMLN 11, CGAA 7.1-.2                       | [1](https://montana.box.com/s/l91d1g3wva43z9qu62w7s5866skbu0dr)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 3/23 | [Delaunay](./notes/2021-03-23.pdf)             |                      |                      | DMLN 12, CGAA 9.1-.2                       | [1](https://montana.box.com/s/xk0jccpjh47k0nxe8ww5a6umhcew259y)    |
| 3/25 | [Delaunay RIC](./notes/2021-03-25.pdf)         |                      | [HW 05](./hw/05.pdf) | DMLN 13, CGAA 9.3-.4                       | [1](https://montana.box.com/s/jaz8nawkjk4zgw3tn5mz97usldxx6hid)    |
|      |                                                |                      |                      |                                            |                                                                    |
| 3/30 | [Hulls/Env/DT/Vor](./notes/2021-03-30.pdf)     |                      |                      | DMLN L16, CGAA 11.5                        | [1](https://montana.box.com/s/25u1dq4v9bsvim1c7m2vyb2rny36zn6i)    |


### April

| Date | Description                                    | Assigned             | Due                  | Proj | Recommended Reading                        |
|------|------------------------------------------------|----------------------|----------------------|------|--------------------------------------------|
| 4/01 | Exam 2                                         |                      |                      |      |                                            |
|      |                                                |                      |                      |      |                                            |
| 4/06 | Arrangements 1                                 |                      |                      |  X   |                                            |
| 4/08 |                                                |                      |                      |  X   |                                            |
|      |                                                |                      |                      |      |                                            |
| 4/13 |                                                |                      |                      |      |                                            |
| 4/15 |                                                |                      |                      |  X   |                                            |
|      |                                                |                      |                      |      |                                            |
| 4/20 |                                                |                      |                      |      |                                            |
| 4/22 |                                                |                      |                      |  X   |                                            |
|      |                                                |                      |                      |      |                                            |
| 4/27 | Finals week                                    |                      |                      |  X   |                                            |
| 4/29 | Finals Week                                    |                      |                      |  X   |                                            |

### Potential Upcoming Topics:

- Arrangements (DMLN L14, CGAA 8.3 / DMLN L15, CGAA 8.4)
- Motion Planning (DMLN L18, CGAA 13)
- Range searching
- Well separated pair decomposition
- Geometric sampling
- Cake Cutting
- Approximate Nearest Neighbors
- Curve & Surface Reconstruction
- Meshing

## Evaluation

Your grade for this class will be determined by:

* 30% [Group Project](./hw/proj.pdf)
* 40% [Homework](./hw/) (lowest homework is dropped)
* 15% Exam 1
* 15% Exam 2

## Policies

### Attendance

Attendance in class with not be taken but students are responsible for all
material covered in class.  Attendance is strongly recommended.

### Assignments

There will be regular homework assignments (about every other week) consisting
of written problems (and possibly a few coding exercises).  Homeworks will be
posted in the schedule.  Solutions should be submitted as a PDF on Brightspace.
(The tool that I use for grading papers only works with PDFs, so any file format
other than PDF will receive a 0.) Homework is due at 23:59 on the due date. Late
homework will not be accepted.

You do NOT need to write up your solutions with LaTex, but I highly encourage
you to do so.  You can find some resources for getting started with latex (and
for making figures, and keeping all those files safe with git) in the [student
resources repo](https://github.com/compTAG/student-resources).

I encourage collaboration, see collaboration section for details.

I will write assignments in latex and [post the source](./hw/src).

### Discussion

Group discussions, questions, and announcements will take place using Slack. It
is okay to send me a direct message or email if you have a question that you feel
is not appropriate to share with the class.  If, however, you send me an message
with a question for which the response would be useful to the rest of the class,
I will likely ask you to post publicly.

We will use the Computational Topology and Geometry (CompTaG) [slack group](
https://join.slack.com/t/tda-at-msu/shared_invite/zt-3t3bpyz6-VoD~75dH6NwqMzXeZ9Szqg).
Please join the group and join the #csci-534-sp21 channel and #seminar (you do
not need to attend seminar, but keep an eye on the channel for interesting
talks).
There are lots of other
discussions and announcements going on in the group for various CompTaG
projects.  Please hop on #announcements and say "Hi!" to the group.  Feel free
to poke into the various public groups, listen quietly or get involved in the
conversation.

### Collaboration

Collaboration IS encouraged, however, all submitted individual work must be your
own and you must acknowledge your collaborators at the beginning of the
submission.

On any group project, every team member is expected to make a substantial
contribution. The distribution of the work, however, is up to the team.

A few specifics for the assignments.  You may:

* Work with anyone in the course.
* Share ideas with others in the course
* Help other teams debug their code or proofs.

You may NOT:

* Submit a proof or code that you did not write.
* Modify another's proof or code and claim it as your own.

Using resources in addition to the course materials is encouraged. But, be sure
to properly cite additional resources. Remember, it is NEVER acceptable to pass
others work off as your own.

Paraphrasing or quoting another's work without citing the source is a form of
academic misconduct. Even inadvertent or unintentional misuse or appropriation
of another's work (such as relying heavily on source material that is not
acknowledged) is considered plagiarism. If you have any questions about using
and citing sources, you are expected to ask for clarification. My rule of thumb
is if I am in doubt, I cite.

By participating in this class, you agree to abide by the [student code of
conduct](http://www.montana.edu/policy/student_conduct/).  Please review the
policy.


### Classroom Etiquette

Please, keep your mics muted, when you are not speaking. Background noise from
your surrounds can be destructing to other learners. Disruptions to the class
will result in you being asked to leave the lecture and will negatively impact
your grade.


### Health-Related Class Absence

Please evaluate your own health status regularly and refrain from attending
class and other on-campus events if you are ill. MSU students who miss class due
to illness will be given opportunities to access course materials online. You
are encouraged to seek appropriate medical attention for treatment of illness.
In the event of contagious illness, please do not come to class or to campus to
turn in work or attend class. Instead notify me over slack about your absence
as soon as practical, so that accommodations can be made. Please note that
documentation (a Doctor's note) for medical excuses is not required. MSU
University Health Partners - as part their commitment to maintain patient
confidentiality, to encourage more appropriate use of healthcare resources, and
to support meaningful dialogue between instructors and students - does not
provide such documentation.

### Disabilities

If you are a student with a disability and wish to use your approved
accommodations for this course, please contact me during my office hours to
discuss. Please have your Accommodation Notification or Blue Card available for
verification of accommodations. Accommodations are approved through the Office
of Disability Services located in SUB 174. www.montana.edu/disabilityservices

## Additional Happenings

Want to learn even more about computational geometry?! While not in any way
required as part of the class, please, feel free to participate in any of the
fun happenings of the [CompTaG](https://www.cs.montana.edu/comptag/) research
group!  We are a very active group and there are lots of opportunities for you
to get involved if you would like.  All events take place over Zoom.

* Every Mon 15:10-16:00 CompTaG hosts a research seminar.  We cover interesting
  research papers.  Usually, we cover about 1 paper every 2-3 weeks, but focus
  on understanding content over covering a lot of material.  Feel free to join
  up or enrolls in CSCI X94 for credit. [Zoom
  Link](https://us02web.zoom.us/j/87358801902?pwd=WEh6WUozYW1PeUFNWXNSQThSL0Q1Zz09)

You can also check out research papers.  Some of the best conferences are:

* Symposium on Computational Geometry (SoCG)
* Symposium on Discrete Algorithms (SoDA)
* Symposium on Theory of Computing (STOC)
* Foundations of Computer Science (FoCS)
* European Symposium on Algorithms (ESA)

But, let me know if you have a specific interest and I can point you in a
direction to help you get started.
