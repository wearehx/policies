# HX Administration Policy

## Introduction

This posts documents how the HX group will be run and administered. The policies in this document of a common theme of accountability and transparency. We believe that posts should only be deleted under certain circumstances, and all logs of what the admins are doing and discussing should be public.

## Management of Administration

- We will increase the number of admins per term as the current admin team sees fit. This will not be based on any ratios (i.e. 1 admin per 500 users), but based on how many bad posts are getting by unmoderated. If all bad posts are caught within some small amount of time (i.e. 30 minutes) of posting, then we have enough admins
- The length of a term for an admin will be 3 months
- An admin can serve for a maximum of two consecutive terms, but there is no maximum limit on the number of terms an admin can serve for
- All admin activity will be public. In the case of bans, see the ban policy later in this document. For larger, more official meetings, either the entire chat log will be posted (possibly as a Github commit or a gist), or paraphrased meeting minutes. Small, one-off conversations/meetings do not need to be public.

## Election of Admins

- The current admin team will determine how many admins are elected for the next term. 
- 14 days before the end of a term, the web interface will allow candidates to mark themselves as running. 
  - Candidates must be nominated by three group members via the web interface (after they have marked themselves as running) to be put on the ballot. Each group member can nominate one member per term.
- 7 days before the end of a term, the web interface will allow group members to vote for a candidate. 
- Votes will stop being accepted after 11:59PM GMT on the day the term ends. The current admins will use the voting result to add/remove themselves, if needed.
- The voting system will publish a freely downloadable list of UUIDs and their vote after votes stop being accepted.

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

Note that there are many tasks such as Hackbot administration, Github projects, etc. that do not need to be solely managed by admins.

## Post deletion

We believe that posts should only be deleted in a few specific cases. First of all, any spam from hacked accounts or bots will be deleted. Second, any posts violating Facebook's content policies will also be deleted. Finally, content can be deleted by an admin if the content is harassing a *specific* user, and that user requests that the content be removed. Note that generally objectionable content that does not target a *specific* user will not be removed (unless it violates Facebook's content policies), and will only be closed instead.

All other content will be closed. The reason for this is to provide transparency as to what the admins deem to be bad content, and to leave examples of bad content in the group in an "archived" state so they can be used as examples of what not to post, as well as serving as precedent for closing future bad posts.

## Ban Policy

You may be banned by violating any of the rules defined in the content policy. A warning may be given first depending on the which policy was violated and the severity of the violation.

When a user is banned, they have a chance to return to the group. They must make a post in Hackers
Ban Appeals (not created yet), to argue why they shouldn’t be banned, or to apologize and request that they be re-added. If the user is not apologetic or we (the admins) and the community (jointly) do not agree with the user’s justification for their behavior, they will be banned from Hackers Ban Appeals and no further appealing can take place. Further policy violations in the main group after being re-added will result in immediate ban from both groups with no chance of appealing.

The purpose of this process is both to give users a second chance, and to have a public space to discuss whether the actions of an admin were justified. Thus, it will not be possible for admins to silently ban individuals for no reasons. If an admin does this and immediately bans the user from the appeals group as well, the admin who did this will be immediately removed from their position as soon as this comes to light in the main group (which can be done by another member).

## GitHub

[TODO: Ian, fill this in]
