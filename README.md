# Gitlab APIs (V4) - Postman_collection

<div align="center">
  <img src="MEDIA/gitlab_api.png">
</div>

<br>

## Usage

- Open [Postman](https://www.postman.com/) and hit `Import`, next to the `workspace` in which you'd like to have such collection;<br><br>
- Upload the `api_v4_collection.json` collection and begin to use it right away!<br><br>
- Create two `environments` - one for `Gitlab Sandbox`, another for `Gitlab Production`, fill in the ENV vars for your own domains (within an ENV var named `CI_API_V4_URL` - use the same var name within each `environment`) and for authorization (within an ENV var named `ACCESS_TOKEN` - use the same var name within each `environment`) towards such domains and then test your infrastructures by easily switching between the environments created. This way, the present collection, powered by Postman, would know to fill in those two ENV vars within every API that would need those, leaving you only the custom options to complete the APIs with company-proprietary information, such a specific `commit_sha`, `project_id`, etc., per your own needs, considering the specific APIs used.

<br>

## Which API Schemas can be found in here?

`Note:` It's not complete, but contains the most used APIs. You can extend over it!

🟩 BRANCHES <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Branches<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Branch<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Branch<br>
&emsp;&emsp;🟠
 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Branch<br>
&emsp;&emsp;🟠
 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Merged Branches<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Protected Branches<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Protected Branch or Wildcard Branch(es) Protection<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Protected Branch(es)<br>
&emsp;&emsp;🟤 `PATCH` Protected Branch<br>
&emsp;&emsp;🟠
 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Unprotected Branch(es)<br>

🟩 COMMITS <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Commits<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Commit<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Commit's References<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Commit's Diff<br>

🟩 GROUPS <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Groups<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group by ID<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group(s) by Name<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Group<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Group<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Subgroups<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Descendent Groups<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Projects<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Shared Projects<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Push Rules<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's Members<br>
&emsp;&emsp;🟣 `PUT` &nbsp;&nbsp;&nbsp;&nbsp;Member's Access<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Member<br>

🟩 PROJECTS <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Projects<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project by ID<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project(s) by Name<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project's Users<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project's Members<br>
&emsp;&emsp;🟣 `PUT` &nbsp;&nbsp;&nbsp;&nbsp;Member's Access<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Member<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project's Push Rules<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Trigger Tokens<br>

🟩 MERGE REQUESTS <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Merge Request<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Project's MRs<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Group's MRs<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Commit's MRs<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Merge Request's Diffs<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Merge Request<br>
&emsp;&emsp;🟣 `PUT` &nbsp;&nbsp;&nbsp;&nbsp;Merge a Merge Request<br>

🟩 PIPELINES <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Pipelines<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Pipeline<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Pipeline<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Pipeline<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Latest Pipeline<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scheduled Pipelines<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scheduled Pipeline<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Retry Pipeline's Jobs<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Cancel a Pipeline<br>

🟩 SEARCH <br>
&emsp;&emsp;🟩 ADVANCED SEARCH <br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: projects<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: issues<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: merge requests<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: milestones<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: snippet titles<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: users<br>

&emsp;&emsp;🟩 GROUP SEARCH <br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: projects<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: issues<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: merge requests<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: milestones<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: users<br>

&emsp;&emsp;🟩 PROJECT SEARCH <br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: issues<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: merge requests<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: milestones<br>
&emsp;&emsp;&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Scope: users<br>

🟩 TAGS <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Tags<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Tag<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Tag<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Tag<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Protected Tags<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Protected Tag<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Protect Tag(s)<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Unprotect Tag(s)<br>

🟩 VARIABLES (Group) <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Variables<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟣 `PUT` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>

🟩 VARIABLES (Project) <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Variables<br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟡 `POST` &nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟣 `PUT` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>
&emsp;&emsp;🟠 `DEL` &nbsp;&nbsp;&nbsp;&nbsp;Variable<br>

🟩 VERSION (of Gitlab) <br>
&emsp;&emsp;🟢 `GET` &nbsp;&nbsp;&nbsp;&nbsp;Version<br>
