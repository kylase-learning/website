{% macro show_main_text() %}
<div id="main">

Here is a list of main deliverables of the project; their details are given in the subsequent sections.
* Product
  * [Executable](#deliverable-executable)
  * [Source code](#deliverable-source-code)
* Documentation
  * [User Guide](#deliverable-user-guide-ug)
  * [Developer Guide](#deliverable-developer-guide-dg)
  * [Product Website](#deliverable-product-website)
  * [Project Portfolio Page](#deliverable-project-portfolio-page-ppp)
* [Product Demo](#deliverable-demo)
* [Practical Exam Dry Run](#deliverable-practical-exam-dry-run)
* [Practical Exam](#deliverable-practical-exam)
  * Peer testing results
  * Peer evaluation


### Deliverable: Executable
<span id="project-deliverables-executable">

* The product should be delivered as an executable jar file.
* Ideally, the product delivered at v1.4 should be a <tooltip content=" i.e., it can be used by end-users">_releasable_</tooltip> product. However, in the interest of lowering your workload, we do not penalize if the product is <tooltip content="i.e., the product is not usable by end-users because some essential features are missing">not releasable</tooltip>, ==as long as the product is <tooltip content="i.e., the features it has can be tested from an end-user perspective">_acceptance testable_</tooltip>==.
</span>

### Deliverable: Source code
<span id="project-deliverables-sourcecode">

* The source code should match the executable, and should include the revision history of the source code, as a Git repo.
</span>


### Deliverable: User Guide (UG)
<span id="project-deliverables-ug">

* The User Guide (UG) of the product should match the proposed v2.0 of the product and in sync with the current version of the product.
* Features not implemented yet should be clearly marked as `Coming in v2.0`
* Ensure the UG matches the product precisely, as it will be used by peer testers (and ==any inaccuracy in the content will be considered bugs==).
</span>


### Deliverable: Developer Guide (DG)
<span id="project-deliverables-dg">

* The Developer Guide (DG) of the product should match the proposed v2.0 of the product and should be in sync with the current version of the product.
* {{ icon_important_big_red }} **The appendix named _Instructions for Manual Testing_** of the Developer Guide should include testing instructions to **cover the features of each team member**. There is no need to add testing instructions for existing AB3 features if you did not touch them.<br>
  {{ icon_tip }} What to include in the appendix _Instructions for Manual Testing_? This appendix is meant to give some guidance to the tester to chart a path through the features, and provide some important test inputs the tester can copy-paste into the app. There is no need to give a long list of test cases including all possible variations. It is upto the tester to come up with those variations. However, if the instructions are inaccurate or deliberately misses/mis-states information to make testing harder %%i.e. annoys the tester%%, the tester can report it as a bug %%(because flaws in developer docs are considered as bugs)%% or give a lower rating for the _testability_ of your product.
* Ensure the DG parts included in PPPs match the product precisely, as PPPs will be used by peer evaluators (and ==any inaccuracy in the content will be considered bugs==).
    
</span>


### Deliverable: Product Website
<span id="project-deliverables-website">

* Include an updated version of the online UG and DG that match v1.4 executable
* **README** :
  * ==Ensure the `Ui.png` matches the current product==
<div class="indented-level3" id="tips-for-product-screenshot">

<box>

{{ icon_tip }} **Some common sense tips for a good product screenshot**

`Ui.png` represents your product in its full glory.
* Before taking the screenshot, populate the product with data that makes the product look good. For example, if the product is supposed to show photos, use real photos instead of dummy placeholders.
* It should show a state in which the product is well-populated %%i.e., don't leave data panels largely blank%%
* Choose a state that showcase the main features of the product %%i.e., the login screen is not usually a good choice%%
* Avoid annotations (arrows, callouts, explanatory text etc.); it should look like the product is in use for real.

<panel type="seamless" header="Examples" expanded >

<tabs>
  <tab header=":-1: Not Good">

Reason: Distracting annotations.

   <img src="images/Ui-notGood1.png" width="600" />

  </tab>
  <tab header=":-1: Not Good">

Reason: Not enough data.

   <img src="images/Ui-notGood2.png" width="600" />

  </tab>
  <tab header=":+1: Good">

   <img src="images/Ui-good1.png" width="600" />

  </tab>
  <tab header=":+1: Good">

   <img src="images/Ui-good2.png" width="600" />

</tab>
</tabs>

</panel>

</box>
</div>

* **AboutUs** : Ensure the following:
  * Use a suitable profile photo
<div id="profile-photo" class="indented-level2">

* The purpose of the profile photo is for the teaching team to identify you. Therefore, choose a recent individual photo showing your face clearly (i.e., not too small) -- somewhat similar to a passport photo. Some examples can be seen in the 'Teaching team' page. Given below are some examples of good and bad profile photos.<br>
  <img src="{{baseUrl}}/admin/images/profilephotos.png" style="width: 365.33px">

* If you are uncomfortable posting your photo due to security reasons, you can post a lower resolution image so that it is hard for someone to misuse that image for fraudulent purposes. If you are concerned about privacy, you may use [a placeholder image](https://en.wikipedia.org/wiki/File:Portrait_placeholder.png) in place of the photo in module-related documents that are publicly visible.

</div>

  * Contains a ==link to each person's Project Portfolio page== 
  * Team member ==names match full names used by LumiNUS==
  
    
</span>

### Deliverable: Project Portfolio Page (PPP)
<span id="project-deliverables-ppp">

At the end of the project each student is required to submit a _Project Portfolio Page_.

* **Objective:** 
  * For you to use %%(e.g. in your resume)%% as a well-documented data point of your SE experience 
  * For us to use as a data point to evaluate your,
    * contributions to the project
    * your documentation skills

* **Sections to include:**
  * **Overview**: A short overview of your product to provide some context to the reader.
  * **Summary of Contributions**:
    * **Code contributed**: Give a link to your code on [Project Code Dashboard](https://nus-{{ module | lower }}-{{ semester | lower }}.github.io/{{ module | lower }}-dashboard), which should be `https://nus-{{ module | lower }}-{{ semester | lower }}.github.io/{{ module | lower }}-dashboard/#=undefined&search=githbub_username_in_lower_case` (==replace `githbub_username_in_lower_case` with your actual username== in lower case e.g., `johndoe`). This link is also available in the [Project List Page]({{baseUrl}}/admin/projectList.html) -- linked to the :fas-code: icon under your photo.
    * **Features implemented:** A summary of the features you implemented. If you implemented multiple features, you are recommended to indicate which one is the biggest feature.
    * **Other contributions:**
      * Contributions to project management %%e.g., setting up project tools, managing releases, managing issue tracker etc.%%
      * Evidence of helping others %%e.g. responses you posted in our forum, bugs you reported in other team's products%%,
      * Evidence of technical leadership %%e.g. sharing useful information in the forum%%

  * **Contributions to the User Guide**: Reproduce the parts in the User Guide that you wrote. This can include features you implemented as well as features you propose to implement.<br>
    %%The purpose of allowing you to include _proposed_ features is to provide you more flexibility to show your documentation skills. e.g. you can bring in a proposed feature just to give you an opportunity to use a UML diagram type not used by the actual features.%%
  * **Contributions to the Developer Guide**: Reproduce the parts in the Developer Guide that you wrote. Ensure there is enough content to evaluate your technical documentation skills and UML modelling skills. You can include descriptions of your design/implementations, possible alternatives, pros and cons of alternatives, etc.

  * If you plan to use the PPP in your Resume, you can also include your SE work outside of the module (will not be graded)

* **Format**:
  * File name: `docs/team/githbub_username_in_lower_case.adoc` e.g., `docs/team/johndoe.adoc`
  * {{ icon_example }} Follow the [example in the AddressBook-Level3](https://nus-{{ module | lower }}-{{ semester | lower }}.github.io/addressbook-level3/team/johndoe.html)

  * {{ icon_tip }} You can use the [Asciidoc's `include` feature](http://asciidoctor.org/docs/asciidoc-syntax-quick-reference/#include-files) to include sections from the developer guide or the user guide in your PPP. Follow the example in the [sample](https://nus-{{ module | lower }}-{{ semester | lower }}.github.io/addressbook-level3/team/johndoe.html).

  * =={{ icon_important_big_red }} It is assumed that all contents in the PPP were written primarily by you.== If any section is written by someone else %%e.g. someone else wrote the description of your feature in the User Guide%%, clearly state that the section was written by someone else %%(e.g. `Start of Extract [from: User Guide] written by Jane Doe`)%%. %%Reason: Your writing skills will be evaluated based on the PPP%%

* **Page limit**:
  Content | Limit
  ------- | -----
  Overview + Summary of contributions | 0.5-1 (soft limit)
  Contributions to the User Guide | 1-3 (soft limit)
  Contributions to the Developer Guide | 3-6 (soft limit)
  Total | 5-10 ==(strict)==

  * The ==page limits given above are _after_ converting to PDF format==. The actual amount of content you require is actually less than what these numbers suggest because the HTML → PDF conversion adds a lot of spacing around content.
  * %%Reason for page limit: These submissions are peer-graded (in the PE) which needs to be done in a limited time span.%%<br>
   If you have more content than the limit given above, you can give a representative samples of UG and DG that showcase your documentation skills. Those samples should be understandable on their own. For the parts left-out, you can give an abbreviated version and refer the reader to the full UG/DG for more details.<br>
   %%It's similar to giving extra details as appendices; the reader will look at the UG/DG if the PPP is not enough to make a judgment. For example, when judging documentation quality, if the part in the PPP is not well-written, there is no point reading the rest in the main UG/DG. That's why you need to put the most representative part of your writings in the PPP and still give an abbreviated version of the rest in the PPP itself. Even when judging the quantity of work, the reader should be able to get a good sense of the quantity by combining what is quoted in the PPP and your abbreviated description of the missing part. There is no guarantee that the evaluator will read the full document.%%


</span>

### Deliverable: Demo
<span id="project-deliverables-demo">

* **Duration:** Strictly 18 minutes for a 5-person team and 15 minutes for a 4-person team. Exceeding this limit will be penalized. Any set up time will be taken out of your allocated time.

* **Target audience**: Assume you are giving a demo to a higher-level manager of your company, to brief him/her on the current capabilities of the product. This is the first time they are seeing the new product you developed but they are familiar with the AddressBook-level3 (AB3) product. The actual audience are the evaluators (the team supervisor and another tutor).

* **Scope**: 
  * **Each person should demo the enhancements they added**. However, it's OK for one member to do all the typing.
  * Each person should demo their part in one go %%i.e., one person should not appear multiple times in the demo. Reasons: it will interfere with grading as some things are graded individually%%. However, it's OK for one person to give a short intro at the start and appear again later in the demo to demo her features.
  * Subjected to the previous two points, as far as possible, organize the demo to present a cohesive picture of the product as a whole, presented in a logical order. %%Remember to explain the profile of the target user profile and value proposition early in the demo.%%
  * It is recommended you showcase how the feature improves the user’s life rather than simply describe each feature.
  * No need to cover design/implementation details as the manager is not interested in those details.
  * Do not demo features you inherited from AB3 unless they are needed to explain your new features. %%Reason: existing features will not earn you marks, and the audience is already familiar with AB3 features.%%
  * Plan the demo to be in sync with the impression you want to create. For example, if you are trying to convince that the product is easy to use, show the easiest way to perform a task before you show the full command with all the bells and whistles.

* **Structure:**
  * Demo the product using the same executable you submitted, on your own laptop, using the TV.  
  * It can be **a _sitting down_ demo**: You'll be demonstrating the features using the TV while sitting down. But you may stand around the TV if you prefer that way.
  * It will be an uninterrupted demo: The audience members will not interrupt you during the demo. That means you should finish within the given time.
  * The demo should use a sufficient amount of <tooltip content="`Mr aaa` is not a realistic person name">_realistic_</tooltip> demo data. %%e.g at least 20 contacts%%. Trying to demo a product using just 1-2 sample data creates a bad impression.
  * **Dress code** : The level of formality is up to you, but it is recommended that the whole team dress at the same level.

* **Optimizing the time:** 
  * Spend as much time as possible on demonstrating the actual product. Not recommended to use slides (if you do, use them sparingly) or videos or lengthy narrations.  
   Avoid skits, re-enactments, dramatizations etc. This is not a sales pitch or an informercial. While you need to show how a user use the product to get value, but you don’t need to act like an imaginary user. For example,<br>
   [Instead of this] `Jim get’s a call from boss. "Ring ring", "hello", "oh hi Jim, can we postpone the meeting?" "Sure". Jim hang up and curses the boss under his breath. Now he starts typing ..etc.`<br>
   [do this] `If Jim needs to postpone the meeting, he can type …`<br>
    It’s not that dramatization is bad or we don’t like it. We simply don’t have enough time for it.  
    Note that CS2101 demo requirements may differ. Different context → Different requirements.  
  * Rehearse the steps well and ensure you can do a smooth demo. Poor quality demos can affect your grade.
  * Don’t waste time repeating things the target audience already knows. e.g. no need to say things like "We are students from NUS, SoC". 

* **Special circumstances:**
  * If a significant feature was not merged on time: inform the tutor and get permission to show the unmerged feature using your own version of the code. Obviously, unmerged features earn much less marks than a merged equivalent but something is better than nothing.
  * If you have no user visible features to show, you can still contribute to the demo by giving an overview of the product (at the start) and/or giving a wrap of of the product (at the end).
  * If you are unable to come to the demo due to a valid reason, you can ask a team member to demo your feature. Remember to submit the evidence of your excuse %%e.g., MC%% to prof. The demo is part of module grading and ==absence without a valid reason== will cause you to lose marks.

</span>

### Deliverable: Practical Exam (Dry Run)

<span id="project-deliverables-practicalexam-dry-run">

**What**: The v1.3 is subjected to a round of peer _acceptance/system testing_, also called the _Practical Exam Dry Run_ as this round of testing will be similar to the graded <trigger trigger="click" for="modal:projectDeliverablesPeDryRun-pe">Practical Exam that will be done at v1.4</trigger>.

**When, where**: uses a 30 minute slot at the start of week 11 lecture

<modal large title="Admin {{ icon_embedding }} Project → Deliverables → Practical Exam" id="modal:projectDeliverablesPeDryRun-pe">
  <include src="project-deliverables.md#project-deliverables-practicalexam"/>
</modal>

{{ icon_important_big_red }} **Grading**: Taking part in the PE dry run is strongly encouraged as it ==can affect your grade in the following ways==.
* If the product you are allocated to test in the Practical Exam (at v1.4) had a very low bug count, we will consider your performance in PE dry run as well when grading the PE.
* PE dry run will help you practice for the actual PE.
* Taking part in the PE dry run will earn you participation points.
* There is ==no penalty for bugs reported== in your product. Every bug you find is a win-win for you and the team whose product you are testing.

**Objectives**:
* **To train you** to do manual testing, bug reporting, bug <tooltip content="assigning of priority order">triaging,</tooltip> bug fixing, communicating with users/testers/developers, evaluating products etc.
* **To help you improve your product** before the final submission.

<include src="project-testing.mbdf#testingPreparations" />

**During the session**:
1. **Take note of your team to test**. Distributed via LumiNUS gradebook and via email.
1. Download the latest jar file from the team's GitHub page. ==Copy it to an empty folder==.
1. Confirm you are testing the allocated product by comparing the product UI with the UI screenshot sent via email.

<div id="project-deliverables-pe-testing-intructions">
<box>

##### Testing instructions for PE and PE Dry Run

* **What to test**:
  * PE Dry Run (at **v1.3**):
    * Test the product ==based on the User Guide== (the UG is most likely accessible using the `help` command).
    * Do ==_system_ testing first== %%i.e., does the product work as specified by the documentation?%%. If there is time left, you can ==do _acceptance_ testing as well== %%i.e., does the product solve the problem it claims to solve?%%.
  * PE (at **v1.4**):
    * Test ==based on the Developer Guide== (Appendix named _Instructions for Manual Testing_) ==and the User Guide==. The testing instructions in the Developer Guide can provide you some guidance but if you follow those instructions strictly, you are unlikely to find many bugs. You can deviate from the instructions to probe areas that are more likely to have bugs.
    * As before, do both ==system testing and acceptance testing== but give priority to system testing as system testing bugs can earn you more credit.

* **These are considered _bugs_**:
  * Behavior differs from the User Guide
  * A legitimate user behavior is not handled %%e.g. incorrect commands, extra parameters%%
  * Behavior is not specified and differs from normal expectations %%e.g. error message does not match the error%%
  * The feature does not solve the stated problem of the intended user i.e., the feature is 'incomplete'
  * Problems in the User Guide e.g., missing/incorrect info

* **Where to report bugs**: Post bug in the following issue trackers that you created in your personal GitHub account (==not in the team's repo==):
  * PE Dry Run (at **v1.3**): `pe-d`<br>
  * PE (at **v1.4**): `pe`

* **Bug report format**:
  * {{ icon_important_big_red }} Post bugs as you find them %%(i.e., do not wait to post all bugs at the end)%% because the issue tracker will close exactly at the end of the allocated time.
  * Each bug should be a separate issue.
  * Write good quality bug reports; ==poor quality or incorrect bug reports will not earn credit==.
  * Use a descriptive title.
  * Give a good description of the bug with ==steps to reproduce and screenshots==.
  * Assign a severity to the bug report. Bug report without a priority label are considered `severity.Low` (lower severity bugs earn lower credit)<br>

<div class="indented-level4">
<include src="appendixE-gitHub.md#bug-severity" />
Also assign a `type.*` label to the issue.
<include src="project-deliverables.md#type-labels" />
</div>

* **About posting _suggestions_:**
  * PE Dry Run (at **v1.3**): You can also post suggestions on how to improve the product. {{ icon_tip }} Be diplomatic when reporting bugs or suggesting improvements. For example, instead of criticising the current behavior, simply suggest alternatives to consider.
  * PE (at **v1.4**): Do not post suggestions. But if a feature is missing a critical functionality that makes the feature less useful to the intended user, it can be reported as a bug.

* **If the product doesn't work at all:** If the product fails catastrophically %%e.g., cannot even launch%%, you can test the _fallback_ team allocated to you. But in this case ==you must inform us immediately after the session== so that we can send your bug reports to the correct team.

</box>
</div>

<modal large title="Admin {{ icon_embedding }} Project →" id="modal:v1.3-ppp">
  <include src="project-deliverables.md#project-deliverables-ppp"/>
</modal>

**After the session**:
* We'll transfer the relevant bug reports to your repo over the weekend. Once you have received the bug reports for your product, it is up to you to decide whether you will act on reported issues before the final submission v1.4. For some issues, the correct decision could be to reject or postpone to a version beyond v1.4.
* You can post in the issue thread to communicate with the tester %%e.g. to ask for more info%%, etc. However, the tester is not obliged to respond.
  * {{ icon_tip }} Do not argue with the issue reporter to try to convince that person that your way is correct/better. If at all, you can gently explain the rationale for the current behavior but do not waste time getting involved in long arguments. If you think the suggestion/bug is unreasonable, just thank the reporter for their view and close the issue.

</span>

### Deliverable: Practical Exam

<span id="project-deliverables-practicalexam">

**Objectives:**
* The primary objective of the PE is to ==increase the rigor of project grading==. Assessing most aspects of the project involves an element subjectivity. As the project counts for 50% of the final grade, it is not prudent to rely on evaluations of tutors alone as there can be significant variations between how different tutors assess projects. That is why we collect more data points via the PE so as to minimize the chance of your project being affected by evaluator-bias.
* Note that ==none of the significant project grade components are calculated solely based on peer ratings==. Rather, PE data are mostly used to cross-validate tutors' grades and identify cases that need further investigation. When peer inputs are used for grading, usually they are combined with tutor evaluations with appropriate weight for each. In some cases ratings from team members are given a higher weight compared to ratings from other teams, if that is appropriate.
* As a bonus, PE also gives us an opportunity to evaluate your manual testing skills, product evaluation skills, effort estimation skills etc.
* Note that the PE is not a means of _pitting you against each other_. Developers and testers play for the same side; they need to push each other to improve the quality of their work -- not bring down each other.

**When, where**: Week 13 lecture

{{ icon_important_big_red }} **Grading**:
* Your performance in the practical exam will affect your final grade and your peers, as explained in [_Admin: Project Grading_]({{ baseUrl }}/admin/project-grading.html) section.
* As your submissions can affect the grades of peers, note that we have put in measures to identify insincere/random evaluations and penalize accordingly.

<include src="project-testing.mbdf#testingPreparations" />

**During:** 

1. **Take note of your team to test**. It will be given to you by the teaching team (distributed via LumiNUS gradebook).
1. **Download from LumiNUS all files** submitted by the team %%(i.e. jar file, User Guide, Developer Guide, and Project Portfolio Pages)%% ==into an empty folder==.
1. **[60 minutes] Test the product and report bugs** as described below:

<div class="indented-level2">
  <include src="project-deliverables.md#project-deliverables-pe-testing-intructions" />
</div>

1. **[Remainder of the session] Evaluate the following aspects.** Note down your evaluation in a hard copy (as a backup). Submit via TEAMMATES. You are recommended to complete this during the PE session but ==you have until the end of the day to submit (or revise) your submissions==.
   * **A. Product Design** [{{ icon_team }}]:

<div class="indented-level2">
  <include src="project-grading.md#projectGrading-featureFit-instructions" />
</div>

   * **B. Quality of user docs** [{{ icon_individual }}]:
<div class="indented-level2">
  <include src="project-grading.md#projectGrading-userGuide-instructions" />
</div>

   * **C. Quality of developer docs** [{{ icon_individual }}]:
<div class="indented-level2">
  <include src="project-grading.md#projectGrading-devGuide-instructions" />
</div>

   * **D. Feature Quality** [{{ icon_individual }}]:
<div class="indented-level2">
  <include src="project-grading.md#projectGrading-featureQuality-instructions" />
</div>

   * **E. Amount of work** [{{ icon_individual }}]:
<div class="indented-level2">
  <include src="project-grading.md#projectGrading-effort-instructions" />
</div>

#### Processing PE Bug Reports:

There will be a review period for you to respond to the [bug reports]({{module_org}}/pe-results/issues) you received.

Duration: The review period will start around 1 day after the PE (exact time to be announced) and will last until the following **Wednesday midnight**. However, you are recommended to finish this task ASAP, to minimize cutting into your exam preparation work.

Bug reviewing is recommended to be done as a team as some of the decisions need team consensus.

<box>

**Instructions for Reviewing Bug Reports**

* **First, don't freak out if there are lot of bug reports.** Many can be duplicates and some can be _false positives_. In any case, we anticipate that all of these products will have some bugs and our penalty for bugs is not harsh. Furthermore, it depends on the severity of the bug. Some bug may not even be penalized.

* **Do not edit the subject or the description.** Your response (if any) should be added as a comment.

* You may (but not required to) close the bug report after you are done processing it, as a convenient means of separating the 'processed' issues from 'not yet processed' issues.

* **If the bug is reported multiple times**, mark all copies EXCEPT one as duplicates using the `duplicate` tag (if the duplicates have different severity levels, you should ==keep the one with the highest severity==). In addition, ==use [this technique](https://help.github.com/articles/about-duplicate-issues-and-pull-requests/) to indicate which issue they are duplicates of==.  Duplicates can be omitted from processing steps given below.

* **If a bug seems to be for a different product** (i.e. wrongly assigned to your team), let us know (email prof).

* **Decide if it is a real bug and apply ONLY one of these labels**.

<div class="indented">
<box>

Response Labels:
* `response.Accepted`: You accept it as a bug.
* `response.NotInScope`: It is a valid issue but not something the team should be penalized for %%e.g., it was not related to features delivered in v1.4%%.
* `response.Rejected`: What tester treated as a bug is in fact the expected behavior.  You can reject bugs that you inherited from AB3.
* `response.CannotReproduce`: You are unable to reproduce the behavior reported in the bug after multiple tries.
* `response.IssueUnclear`: The issue description is not clear. Don't post comments asking the tester to give more info. The tester will not be able to see those comments because the bug reports are anonymous.

</box>
</div>

* If applicable, **decide the type of bug**. Bugs without `type.*` are considered `type.FunctionalityBug` by default (which are liable to a heavier penalty).

<div class="indented" id="type-labels">
<box>

**Type** labels:
* `type.FunctionalityBug`: A functionality does not work as specified/expected.
* `type.FeatureFlaw`: One of these:some functionality missing from a feature delivered in v1.4 in a way that the feature becomes less useful to the intended target user for normal usage. i.e., the feature is not 'complete'. In other words, an acceptance testing bug that falls within the scope of v1.4 features. These issues are counted against the 'depth and completeness' of the feature.
* `type.DocTypo`: A minor typo in the documentation %%e.g., spelling error%%. Does not affect the users.
* `type.DocumentationBug`: A flaw in the documentation that can potentially affect the user %%e.g., a missing step, a wrong instruction%%
</box>
</div>

* **If you disagree with the original severity assigned to the bug**, you may change it to the correct level.

{{ icon_important_big_red }} For all cases of downgrading severity or non-acceptance of a bug, ==you must add a comment justifying your stance==. All such cases will be double-checked by the teaching team and indiscriminate downgrading/non-acceptance of bugs without a good justification, if deemed as a case of trying to _game the system_, may be penalized as it is unfair to the tester.

<div class="indented">
  <include src="appendixE-gitHub.md#bug-severity" />
</div>

* **Decide who should fix the bug**. Use the `Assignees` field to assign the issue to that person(s). There is no need to actually fix the bug though. It's simply an indication/acceptance of responsibility. **If there is no assignee, we will distribute the penalty for that bug (if any) among all team members.**
 * We recommend (but not enforce) that the feature owner should be assigned bugs related to the feature, even if the bug was caused indirectly by someone else. Reason: The feature owner should have defended the feature against bugs using automated tests and defensive coding techniques.

* **Add an explanatory comment** explaining your choice of labels and assignees.

* Choose the correct `type.*`, `severity.*` labels and assignee even for bugs you are not accepting. Reason: your _non-acceptance_ may be rejected by the tutor later, in which case we need to grade it as an accepted bug.

</box>

</span>

</div>
{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-deliverables", show_main_text) }}
