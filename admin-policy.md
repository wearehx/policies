# HX Administration Policy

## Introduction

This posts documents how the HX group will be run and administered. The policies in this document of a common theme of accountability and transparency. We believe that posts should only be deleted under certain circumstances, and all logs of what the admins are doing and discussing should be public.

## Policy Change Approval Process

- The process for changes to this repo should start with either a GitHub issue, a post in HX Meta, or a conversation with an admin in ##hx-admin.
- After the initial discussion in one of the above locations, a PR can be made on this repo, either adding a document or modifying a document. The PR text should contain a detailed, well-thought out description of all of the changes and why they are being made. A post should be made in HX Meta announcing the PR.
- All discussion should happen on this PR, and on no other mediums. The entire community should participate in this discussion, not just the admins. After discussion has died down, the admins can choose to merge/reject a PR. In either case, if there was any opposition or unaddressed points in the comments, the admins *must* address all points and sides of the argument when merging.
- Note that formatting, grammar, or simple clarification PRs do not need to go through this process. They can be made as normal PRs against the repo, and an admin can merge them at any time.
- Any changes to a PR before merging should ideally be made by the author of the PR. Pull requests by others to PRs are generally not allowed. The exception to this is when permission is given by the PR author due to the author being unable to make the discussed changes at that time.
- Note that commits should never be removed from PRs (i.e. through rebasing/squashing), as we would like to preserve the entire history of the PR.

## Management of Administration

- We will increase the number of admins per term as the current admin team sees fit. A general indicator of how many admins are needed is to see how long it takes posts to be moderated. If all bad posts are caught within some small amount of time (i.e. 30 minutes) of posting, then we have enough admins
- The length of a term for an admin will be 3 months
- An admin can serve for a maximum of two consecutive terms, but there is no maximum limit on the number of terms an admin can serve for
- All admin activity will be public. In the case of bans, see the ban policy later in this document. For larger, more official meetings, either the entire chat log will be posted (possibly as a GitHub commit or a gist), or paraphrased meeting minutes. Small, one-off conversations/meetings do not need to be public. Ideally, these meetings should occur in the ##hx-admin IRC channel on Freenode.
- It is *highly* recommended that admins idle on ##hx-admin so that the community can easily have a short discussion or ask questions directly to the admins in a public area, without polluting the main HX group. HX Meta is also alright for this purpose, but an IRC conversation can often provide immediate feedback.

## Election of Admins

- The current admin team will determine how many admins are elected for the next term. 
- 14 days before the end of a term, the web interface will allow candidates to mark themselves as running. 
  - Candidates must be nominated by three group members via the web interface (after they have marked themselves as running) to be put on the ballot. Each group member can nominate one member per term.
- 7 days before the end of a term, the web interface will allow group members to vote for a candidate. 
- Votes will stop being accepted after 11:59PM GMT on the day the term ends. The current admins will use the voting result to add/remove themselves, if needed.
- The voting system will publish a freely downloadable list of UUIDs and their vote after votes stop being accepted.
- The election dates for each year will be January 4th, April 4th, July 4th, and October 4th.

### Voting

- Votes are counted via a voting web interface.
  - In the event the web interface becomes inaccessible while voting is in progress, the voting period and moderation term may be extended to the nearest hour based on the outage length.
- The group will have one official maintainer for the voting web interface.
  - The maintainer can be removed and replaced via an unanimous vote among the current elected admins.
  - The maintainer is responsible for producing the results of the election for each term, ensuring the voting application is secure, and maintaining its reliability. 
    - The maintainer may remove clearly spam candidates, and the current admins may veto any removals.
  - The maintainer must not run in any election they maintain.
- The voting system will not allow non-group members to vote; it may additionally deny some users the ability to vote if the user's account appears fraudulent.
- The voting system will securely generate a v4 UUID for each user after they cast their first vote. When the user votes, their UUID will be stored along with their vote. When the election concludes, the UUID and vote will be published to allow auditing of the results.
- Under this model (to be improved in the future), the maintainer is able to access the database linking votes to people, though the integrity of the results is relatively sound.

## Removal of Admins

Administrators may be removed by an unanimous vote among the other current admins. The current administrators may choose to hold a temporary election or wait until the next election if an administrator is voted out. 

## Purpose of Administration

- Lock/close posts (and remove when content policy specifies).
- Ban users and deal with ban appeals (see the ban policy for more details).
- Manage the group name/cover photo and its promotion.

Note that there are many tasks such as Hackbot administration, GitHub projects, etc. that do not need to be solely managed by admins.

## Deletion of Posts

We believe that posts should only be deleted in a few specific cases. First of all, any spam from hacked accounts or bots will be deleted. Second, any posts violating Facebook's content policies will also be deleted. Finally, content can be deleted by an admin if the content is harassing a *specific* user, and that user requests that the content be removed. Note that generally objectionable content that does not target a *specific* user will not be removed (unless it violates Facebook's content policies), and will only be closed instead.

All other content will be closed. The reason for this is to provide transparency as to what the admins deem to be bad content, and to leave examples of bad content in the group in an "archived" state so they can be used as examples of what not to post, as well as serving as precedent for closing future bad posts.

## Ban Policy

You may be banned by violating any of the rules defined in the content policy. A warning may be given first depending on the which policy was violated and the severity of the violation.

When a user is banned, they have a chance to return to the group. They must make a post in Hackers
Ban Appeals (not created yet), to argue why they shouldn’t be banned, or to apologize and request that they be re-added. If the user is not apologetic or we (the admins) and the community (jointly) do not agree with the user’s justification for their behavior, they will be banned from Hackers Ban Appeals and no further appealing can take place. This will not require a formal voting process, and the admins will have final say about the ban. Further policy violations in the main group after being re-added will result in immediate ban from both groups with no chance of appealing.

The purpose of this process is both to give users a second chance, and to have a public space to discuss whether the actions of an admin were justified. Thus, it will not be possible for admins to silently ban individuals for no reasons. If an admin does this and immediately bans the user from the appeals group as well, the admin who did this will be immediately removed from their position as soon as this comes to light in the main group (which can be done by another member).

## GitHub

Anyone can be given read access to our GitHub organization `wearehx`. The current administration team is always given Owner access on the organization. Other users should retain their previous privileges, but the current administration team has the final say and can make modifications as needed.

Projects must be approved by anyone with Owner access and will be given a team on the organization, if needed. Projects must have a `CONTRIBUTING.md` and `README.md` file to document what the project is and how to contribute. Incomplete projects should be removed after a reasonable amount of time; inactive projects should be removed only if the repository serves no purpose to anyone, even outside the group. Ideally, these projects should be transferred to their original owner's GitHub account as opposed to being deleted.
