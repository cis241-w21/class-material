# Welcome to CIS 241 - System-level Programming and Utilities, Winter 2021

## About the Course

### Course Overview
This course should help acquaint you with:

* Navigating and using a Unix-based OS (primarily Linux)
* Remote access and file transfer for Unix systems
* Linux utilities and scripting
* Git/Github
* Programming with a system-level language (C) and memory management

### Helpful Links

* [Syllabus](syllabus.md)
* [Piazza](https://piazza.com/class/kk2pgnmcqcl5n8) -- also [FAQ about Piazza](piazza-faq.md)
* [PrairieLearn](https://prairielearn.engr.illinois.edu/) - log-in
  using "Google" and use your GVSU gmail account
* [ClassTranscribe](https://classtranscribe.com/offering/2eda65cf-d00f-4a0b-bb00-7bba2f88ccc6) -
  select "Google" sign-in and use your GVSU gmail account
* [GVSU VPN Instructions](https://www.gvsu.edu/it/downloading-installing-and-setting-up-pulse-secure-222.htm)

### Need Help?
If you have questions, please ask!  I'm here to help -- it'll
just take place in a virtual format.  I welcome students
to just sign-on to the office hour zoom calls and use the time
to work on their projects and listen to questions others might have.

### COVID
Unfortunately, this will not be a typical semester.  This course
will be entirely online, but there will still likely be
surprises and we will need to be flexible to accommodate changes.

I recognize the difficulties some of you may face.
My goal is to make this semester as effective and as smooth
as possible.  Please reach out to me early and keep me informed
of any issues that arise.

### Course Schedule
This table will have all of the lecture video links, due dates, etc.
added throughout the semester.  Material will be added on a weekly basis.
Lecture video links will be posted under the topic column and released
at the start of each week.

| Week | Date          | Topics | Activities | TODOs |
| ---- | ------------- | ------ | ---------- | --------- |
|  01  | 01/18-01/22 | intro [video](https://classtranscribe.com/video?id=c1de6e62-c98f-4899-9772-35add7fe70e0) <br> ssh (Optional) [video](https://classtranscribe.com/video?id=a8f032d1-09c8-4740-9e61-0be5611a6654) [slides](lec-notes/lec01-intro-ssh.pdf) <br> navigating linux [video](https://classtranscribe.com/video?id=74811691-a0a1-4b97-8650-d7a381f958e1) [slides](lec-notes/lec02-linux-filesystem-basics.pdf)  <br> viewing files [video](https://classtranscribe.com/video?id=47b56232-1d5c-4c8a-8f78-3982a03b1dd1) [slides](lec-notes/lec03-viewing-files.pdf) <br> file transfer [video](https://classtranscribe.com/video?id=f82ca560-7708-4204-8687-a6e41b563043) [slides](lec-notes/lec04-scp-rsync.pdf)  | [minilab 0](minilabs/minilab00.md) | Create a [Piazza account](https://piazza.com/class/kk2pgnmcqcl5n8) <br> Create a [github](https://github.com/) account (if you do not already have one) <br> [Course Survey due Monday 01/25](https://forms.gle/V9LwBgupHKmW19186) <br> Windows Users Only:  [Enable the Linux Subsystem](wsl-guide.md) by Wed 01/20 |
|  02  | 01/25 - 01/29 | sshkeys [video](https://classtranscribe.com/video?id=8c240760-bbbf-4cf2-be22-a5413b148f2a) [slides](lec-notes/lec05-sshkeys-sshaliases.pdf) <br> script/history [video](https://classtranscribe.com/video?id=068ca65e-35fe-446f-aae5-a9124421ff30) [slides](lec-notes/lec06-history.pdf) <br> IO redirection [video](https://classtranscribe.com/video?id=11d4ce0d-ed37-4655-94d5-8033c411d42f) [slides](lec-notes/lec07-redirection.pdf) <br> linux utilities [video](https://classtranscribe.com/video?id=98ba84fd-7258-451a-891e-d74759905aae) [slides](lec-notes/lec08-cut-tr-wc.pdf) | [minilab 1](minilabs/minilab01.md) | - |
|  03  | 02/01 - 02/05 | compression [video](https://classtranscribe.com/video?id=88ceb63c-5d19-4145-93ca-06d7fa6506b6) [slides](lec-notes/lec09-compression.pdf) [files](misc-files/week03/compression) <br> diff/piping [video](https://classtranscribe.com/video?id=b0b2129a-67e4-41d8-8182-c2165c75bc84) [slides](lec-notes/lec10-diff-piping.pdf) [files](misc-files/week03/diff) <br> grep [video](https://classtranscribe.com/video?id=9d4b753d-0aa1-4b50-b1e9-2c8403ae12a6) [slides](lec-notes/lec11-grep-wildcards.pdf) [files](misc-files/week03/grep) <br> git overview [video](https://classtranscribe.com/video?id=881e9710-2f41-4461-972c-ec0f32ae59b3) [slides](lec-notes/lec12-git-overview.pdf) | [minilab 2](minilabs/minilab02.md) |  |
|  04  | 02/08 - 02/12 | git intro [video](https://classtranscribe.com/video?id=c590ff8f-7a26-4743-9add-df5a72a8a4c9) [slides](lec-notes/lec13-git-intro.pdf) <br> git branching [video](https://classtranscribe.com/video?id=e48a0506-df26-469a-8dbb-c077bffa5cdb) [slides](lec-notes/lec14-git-branching.pdf) <br> git remotes [video](https://classtranscribe.com/video?id=a69c17e1-7f00-4d8c-bb54-c986ebeddef3) [slides](lec-notes/lec15-git-remotes.pdf) <br> git merging [video](https://classtranscribe.com/video?id=55eb47cc-7aae-41cb-8207-1fa07d4c2e70) [slides](lec-notes/lec16-git-merging.pdf) | [minilab 3](minilabs/minilab03.md) | [Project 1 Assigned](https://www.prairielearn.org/pl/course_instance/128497/assessment/2309641) |
|  05  | 02/15 - 02/19 | git other [video](https://classtranscribe.com/video?id=ebc71085-1ca2-4b9c-baa9-f1a3dbd4bc43) [slides](lec-notes/lec17-git-other.pdf) <br> vim [video](https://classtranscribe.com/video?id=ea139982-7d96-4f05-a029-e93544173e57) [slides](lec-notes/lec18-vim.pdf) [files](misc-files/week05/vim) <br> permissions/path [video](https://classtranscribe.com/video?id=c7ffd473-eb6c-4035-af25-4b96f9fdafbc) [slides](lec-notes/lec19-permissions-path.pdf) <br> installing from source [video](https://classtranscribe.com/video?id=79af3bd0-16d0-4928-a7b6-3e0c91b05ab7) [slides](lec-notes/lec20-installing-from-source.pdf) <br> processes [video](https://classtranscribe.com/video?id=238ec2bd-c01d-410f-9f93-0cd121c4ca74) [slides](lec-notes/lec21-processes.pdf) | [minilab 4](minilabs/minilab04.md) | Project 1 Due Saturday 02/20 @ 11:59pm <br><br> [Sign-up for Quiz Time Slot](https://docs.google.com/spreadsheets/d/1_wGwc_YFypLKmFRKCPKSWhHj5ol7AAscKBO-awWGttE/edit?usp=sharing) <br> Quiz [Review Guide](misc-files/quiz-review.md) |
|  06  | 02/22 - 02/26 | Bash Scripting <br> basics [video](https://classtranscribe.com/video?id=91542cf6-4f84-41d4-9108-e4aee7e7c814) [slides](lec-notes/lec22-bash-scripting-basics.pdf) [script](misc-files/week06/bash-scripts/basic.sh) <br> arguments [video](https://classtranscribe.com/video?id=647eda3e-b36a-46ff-ab83-5343b9705fba) [slides](lec-notes/lec23-bash-scripting-arguments.pdf) [script](misc-files/week06/bash-scripts/arguments.sh) <br> variables [video](https://classtranscribe.com/video?id=36835a8e-ac0f-40c7-a56a-c6d075fff562) [slides](lec-notes/lec24-bash-scripting-variables-arithmetic.pdf) [script](misc-files/week06/bash-scripts/variables.sh) <br> conditionals [video](https://classtranscribe.com/video?id=10e2208d-771e-416f-83b6-1f58cc476560) [slides](lec-notes/lec25-bash-scripting-conditionals.pdf) [script](misc-files/week06/bash-scripts/conditionals.sh) <br> loops [video](https://classtranscribe.com/video?id=1a488428-4ac1-417e-9378-6790c565b6bd) [slides](lec-notes/lec26-bash-scripting-loops.pdf) [script](misc-files/week06/bash-scripts/loops.sh) <br> arrays [video](https://classtranscribe.com/video?id=dabb2916-5171-44d0-bc54-17cbcf630e06) [slides](lec-notes/lec27-bash-scripting-arrays.pdf) [script](misc-files/week06/bash-scripts/arrays.sh) <br> functions [video](https://classtranscribe.com/video?id=1a1227fd-394b-41a8-a743-065af7571de5) [slides](lec-notes/lec28-bash-scripting-functions.pdf) [script](misc-files/week06/bash-scripts/functions.sh) | [minilab 5](minilabs/minilab05.md) | Command Line Quiz |
|  07  | 03/01 - 03/05 | regex basics [video](https://classtranscribe.com/video?id=d3cb9c39-fe39-427c-a626-afdc54a903b5) [slides](lec-notes/lec29-regex.pdf) <br> regex and grep [video](https://classtranscribe.com/video?id=fd635645-8ee4-412b-89eb-bbd09f5dd74f) [slides](lec-notes/lec30-regex-grep.pdf) <br> sed [video](https://classtranscribe.com/video?id=54f05088-5adb-4f8f-baba-4aa65b59e624) [slides](lec-notes/lec31-sed.pdf) <br> Files: [random files](misc-files/week07) [books](misc-files/written-texts)  | [minilab 6](minilabs/minilab06.md) | Command Line Quiz Retake / Makeup <br> [Project 2 Assigned](https://www.prairielearn.org/pl/course_instance/128497/assessment/2310075)|
|  08  | 03/08 - 03/12 | gawk basics [video](https://classtranscribe.com/video?id=4fd70483-5289-40d7-9489-1f2bd69e0f0d) [slides](lec-notes/lec32-gawk-basics.pdf) [script](misc-files/week08/script-basics.awk) <br> gawk adv [video](https://classtranscribe.com/video?id=684266bc-7be4-400e-8fea-1a194672aa4a) [slides](lec-notes/lec33-gawk-advanced.pdf) [script](misc-files/week08/script-advanced.awk) <br> C intro [video](https://classtranscribe.com/video?id=711bfa10-2296-4571-96e3-7441a89de8ec) [slides](lec-notes/lec34-c-intro.pdf) | [minilab 7](minilabs/minilab07.md) <br> [Solution Video](https://classtranscribe.com/video?id=3a82ae15-a48c-4730-9e48-7fd24a0abae9) | - |
|  09  | 03/15 - 03/19 | C compiling [video](https://classtranscribe.com/video?id=7b7645ec-3fa3-4c8c-bf04-0dcd79536df5) [slides](lec-notes/lec35-c-compiling.pdf) <br> C printing [video](https://classtranscribe.com/video?id=36343308-b4f6-4500-bf0d-79a841141d71) [slides](lec-notes/lec36-c-types-print.pdf) [script](misc-files/week09/types-printing.c) <br> C basics [video](https://classtranscribe.com/video?id=9aba1043-3a71-4df0-ac89-1fbf7b8edd92) [slides](lec-notes/lec37-c-operations-conditionals.pdf) [script](misc-files/week09/ops-cond.c) <br> C loops [video](https://classtranscribe.com/video?id=6b1dff74-7750-46e6-9a68-7abb85d852d5) [slides](lec-notes/lec38-c-loops.pdf) [script](misc-files/week09/loops.c) <br> C pointers [video](https://classtranscribe.com/video?id=8be8a41e-10e8-4fc7-9d6a-5eb0260357c2) [slides](lec-notes/lec39-c-pointers.pdf) [script](misc-files/week09/pointers-intro.c) | [minilab 8](minilabs/minilab08.md) | Project 2 Due Friday 03/19 @ 11:59pm <br> [PL Practice Quiz](https://www.prairielearn.org/pl/course_instance/128497/assessment/2310220) |
|  10  | 03/22 - 03/26 | C stack vs heap [video](https://classtranscribe.com/video?id=235f3ffb-55db-4f53-8f93-6af697dca51f) [slides](lec-notes/lec40-c-stack-heap.pdf) <br> C memory allocation [video](https://classtranscribe.com/video?id=e259913b-6839-45ff-ae78-59ff03d24d17) [slides](lec-notes/lec41-allocating-memory.pdf) [script](misc-files/week10/memory-allocation.c) <br> C arrays & pointers [video](https://classtranscribe.com/video?id=a2b15736-733b-48bd-870f-3b2c7110851b) [slides](lec-notes/lec42-pointers-arrays.pdf) [script](misc-files/week10/pointers-arrays.c)  | [minilab 9](minilabs/minilab09.md) | Midterm Monday 03/22 <br> [Study Guide](misc-files/midterm-recap.md) <br> [Project 3 Released](https://www.prairielearn.org/pl/course_instance/128497/assessment/2310397) |
|  11  | 03/29 - 04/02 | C input [video](https://classtranscribe.com/video?id=fa3c3c7e-e8e3-44ff-b5fd-f706c2be7767) [slides](lec-notes/lec43-c-stdin.pdf) [script](misc-files/week11/reading-input.c) <br> C functions [video](https://classtranscribe.com/video?id=839a1be9-5df7-43eb-aee5-6e0da84d5168) [slides](lec-notes/lec44-c-funcs.pdf) [script](misc-files/week11/functions.c) <br> switch [video](https://classtranscribe.com/video?id=1608ce32-ff0b-4f6d-97ab-0cf9dca38294) [slides](lec-notes/lec45-c-switch.pdf) [script](misc-files/week11/switch.c) <br> header files [video](https://classtranscribe.com/video?id=46004239-92ce-4754-9688-393ff2ef1ada) [slides](lec-notes/lec46-c-header-files.pdf) [files](misc-files/week11/headers) | [minilab 10](minilabs/minilab10.md) | - |
|  12  | 04/05 - 04/09 | 2d arrays - stack, 2d arrays - dynamic allocation, makefiles  | [minilab 11](minilabs/minilab11.md) | Project 3 due Friday 04/09 @ 11:59pm |
|  13  | 04/12 - 04/16 | C string funcs, C mem funcs, gdb/valgrind  |  |  |
|  14  | 04/19 - 04/23 | C arguments, C enums/unions, C fileio, C libraries/misc, Recap  |  |  |
|  15  | 04/26 - 04/30 |  FINAL EXAM Week (Exact Day TBD) |  |  |
