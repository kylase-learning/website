{% from "common/admin.njk" import show_admin_page, show_project_summary_lead with context %}
{% from "common/macros.njk" import embed_topic, thumb, timing_badge with context %}

{% macro show_main_text() %}
<div id="main">

{% call show_project_summary_lead()%}
1. Brainstorm user stories
1. Prioritize user stories
{% endcall %}

<div id="body">

**v1.0 Summary of Milestone**

#### {{ thumb(1) }} Brainstorm user stories

  <img src="{{baseUrl}}/admin/images/v00.png" width="250px">

  Get together with your team members and <trigger trigger="click" for="modal:v10-brainstorming">brainstorm</trigger> for <trigger trigger="click" for="modal:v10-userstories">user stories</trigger> **&nbsp;for the v2.0 of the product**. Note that in the module project you will deliver only up to v1.4 but here you should consider up to v2.0 (i.e. beyond the module).

  * It is ok to have more user stories than you can deliver in the project. %%Aim to create at least 30 user stories. Include all 'obvious' ones you can think of but also look for 'non obvious' ones that you think are likely to be missed by other teams.%%

  * Refer <trigger trigger="click" for="modal:v10-userstoryusagetips">[Textbook {{ icon_embedding }} Specifying Requirements → UserStories →  Usage → (section) Tips]</trigger> for tips on how to use user stories in this task.

  * You can write each user story in a piece of paper (e.g. yellow sticky note, index card, or just pieces of paper about the size of a playing card). Alternatively you can use an online tool (some examples given in <trigger trigger="click" for="modal:v10-onlinetools">[Textbook {{ icon_embedding }} Specifying Requirements → UserStories → Usage → (panel) Tool Examples ]</trigger>).<br>

  * Note that ==you should not 'evaluate' the value of user stories while doing the above==. %%Reason: an important aspect of brainstorming is not judging the ideas generated.%%


<modal large title="Textbook {{ icon_embedding }}" id="modal:v10-brainstorming">
  <include src="../book/gatheringRequirements/brainstorming/unit-inElsewhere-asFlat.md" boilerplate/>
</modal>

<modal large title="Textbook {{ icon_embedding }}" id="modal:v10-userstories">
  <include src="../book/specifyingRequirements/userStories/introduction/unit-inElsewhere-asFlat.md" boilerplate/>
</modal>

<modal large title="Textbook {{ icon_embedding }} Specifying Requirements → UserStories → Usage → (panel)Tool Examples" id="modal:v10-onlinetools">
  <include src="../book/specifyingRequirements/userStories/usage/tools.md"/>
</modal>

<modal large title="Textbook {{ icon_embedding }} Specifying Requirements → UserStories →  Usage → (section) Tips" id="modal:v10-userstoryusagetips">
  <include src="../book/specifyingRequirements/userStories/usage/text.md#usageTips"/>
</modal>

<div class="indented-level3">
<box>

{{ icon_tip }} Recommended: **You can use GitHub issue tracker to manage user stories**, but for that you need to set up your team's GitHub organization, project fork, and issue tracker first. Instructions for doing those steps are in the panel below.

<panel header="%%Admin {{ icon_embedding }} Appendix E: GitHub (extract)%%">
  <include src="appendixE-gitHub.md#organization-setup"/>
  <include src="appendixE-gitHub.md#repo-setup"/>
  <include src="appendixE-gitHub.md#issue-tracker-setup"/>
  <include src="appendixE-gitHub.md#project-schedule-tracking"/>
</panel>

</box>

<panel header="{{ icon_example }} User Story examples (from a different product)" minimized>

`As a user I can add a task by specifying a task description only, so that I can record tasks that need to be done ‘some day’.`
`As a user I can find upcoming tasks, so that I can decide what needs to be done soon.`
`As a user I can delete a task, so that I can get rid of tasks that I no longer care to track.`
`As a new user I can view more information about a particular command, so that I can learn how to use various commands.`
`As an advanced user I can use shorter versions of a command, so that type a command faster.`

</panel>
</div>

<br>

#### {{ thumb(2) }} Prioritize the user stories

  <img src="{{baseUrl}}/admin/images/userstories.png" width="250px">

  Suggested workflow:

  * Take one user story at a time and get team member opinions about it.
  * Based on the team consensus, put the story (i.e. the piece of paper) onto one of these three piles:

    * `Must-Have` : The product will be practically useless to the target user without this feature.
    * `Nice-To-Have` : The target user can benefit from this user story significantly but you are not certain if you'll have time to implement it.
    * `Not-Useful` : No significant benefit to the target user, or does not fit into the product vision.

  * %%If using physical paper to record user stories: After all stories have been put in the above three piles, you can make a record of which stories are in the three piles.%%

</div>
</div>
{% endmacro %}

{{ show_admin_page("project-w05-v10", show_main_text) }}