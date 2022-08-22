## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

---

## ENS Proposal Process


## RFP Overview

ENS DAO operates primarily through "Requests for Proposal" (RFPs). An RFP is a request from the DAO for 
contributors to offer to do work on its behalf, and receive compensation in return.

If you identify a need that you believe you can address, you can write an RFP. Once the RFP is passed, anyone can 
write a proposal in response and be awarded the work. Even if you believe you can do the work yourself, you will 
still need to pass an RFP in order to be awarded the work (and corresponding compensation) by the DAO.

RFPs can be short or long, depending on the project. An RFP for improving the DAO's documentation may only be a 
paragraph or two long, and proposals for it will be equally short. However, an RFP for managing the DAO's funds 
may be lengthy, and a successful proposal could be multiple pages justifying the proposer's ability to take on the job.


    


---
## Evaluation





##### What is the full form of RFP?  

- [ ]  Requests for Payment
- [x]  Requests for Proposal
- [ ]  Requests for Participation
- [ ]  None of the above





##### What is the optimal word length of an RFP?  

- [ ]  One page long
- [ ]  Al-least two pages
- [ ]  Not more than 500 words
- [x]  Anything word length that can justify proposer's ability to take on the job

    


---
## Proposal Process Overview

Proposals follow three basic steps:
1) **Temperature check** - Post to the worksteam’s Temp Check category to get feedback on your idea before creating a 
   formal proposal.
2) **Draft proposal** - Create a draft proposal by creating a new post and selecting the appropriate “Draft Proposals” 
   subcategory. A proposal template will be populated; fill it out, submit it, and solicit feedback on it.

3) **Active Proposal** -  Ask a moderator to move your mature draft to the Active Proposals category and start a vote.


    


---
## Evaluation





##### Select the three basic steps of Proposals  

- [ ]  Proposal Marketing
- [x]  Draft proposal
- [x]  Temperature check
- [x]  Active Proposal

    


---
## Phase 1: Temperature Check — Discourse

The purpose of the Temperature Check is to determine if there is sufficient will to make changes to the status quo.

To create a Temperature Check, ask a general, non-biased question to the community on 
[discuss.ens.domains](https://discuss.ens.domains/) about a potential change (example: “Should ENS decrease 
registration costs for 3-letter domains?”). Forum posts should be in the "DAO-wide -> Temperature Check" category.

Temperature checks are informal and optional; it's up to you to use the feedback to decide if you want to proceed 
further with your proposal.


    


---
## Phase 2: Draft proposal

## RFP Process
1) POST an RFP on the DAO forum with the following information:
    - The need for the RFP
    - Description of work to be done, including scope of work, deliverables, timelines and maximum budget
    - Nomination of a party who will select a winning bid and approve & disburse compensation (the RFP manager)
2) If the stewards agree to adopt your proposal, they will need to decide if it can be paid out of WG funds, or 
   if it requires a DAO-wide vote.
3) If the stewards agree to adopt your RFP, they will decide if it can be paid out of WG funds, or if it needs a DAO wide vote.
      a. If the RFP can be paid out of WG funds, they will set a submission period and post it as an active RFP.
      b. Otherwise, the stewards will create an executable proposal (or, they may ask you to do this). You  will 
         need to specify the actions your proposal will take while it is in draft stage. You may wish to wait 
         until the proposal is stable before doing this. The executable proposal template explains how to do this.


    


---
## Evaluation





##### What is the URL of the ENS community forum?  

- [x]  https://discuss.ens.domains
- [ ]  https://talk.ens.domains
- [ ]  https://gov.ens.domains
- [ ]  https://forum.ens.domains





##### Select the correct option  

- [ ]  Porposals can be paid out of WG funds
- [ ]  Porposals can be paid out of DAO funds
- [x]  Both A and B
- [ ]  Proposals can be only paid out after on-chain voting

    


---
## Phase 2: Draft Executable Proposal

To create a Executable Proposal, [create a new governance proposal](https://github.com/ensdomains/governance-docs/new/main/governance-proposals) 
in the governance-docs repository on GitHub. Start by copying the template for an [executable proposal](executable-proposal-template.md), 
[social proposal](social-proposal-template.md), or [constitutional amendment](constitutional-amendment-template.md), as appropriate. 
Once you have written your proposal, create a Draft Pull Request for it. Start a new post in the DAO-wide -> Draft Proposals" 
category with a link to the PR for discussion.

You will need to specify the actions your proposal will take while it is in draft stage. You may wish to wait until 
the proposal is stable before doing this. The executable proposal template explains how to do this.
      
Once you are confident the proposal is in a stable state, you can proceed to phase 3.


    


---
## Evaluation





##### Select the correct statements for Executable Proposals  

- [ ]  Executable proposals are allways passed via on-chain voting
- [x]  Executable proposals can be passed by Working Gorup Stewards
- [x]  You will need to specify the actions your proposal will take while it is in draft stage
- [ ]  Executable proposals are only needed for changes related to registration fee and duration

    


---
## Phase 3: Active Proposal — Snapshot / Governance Portal

## Proposal Submission for Voting      
Use GitHub to flag your PR as Ready for Review. A contributor will:

1. Merge your PR if it meets the requirements.
2. Assign your proposal a proposal number in the form EP###.
3. Schedule the proposal for a snapshot vote.

If your proposal is a Social Proposal or a Constitutional Amendment, that's it! If the snapshot vote passes, 
the proposal is passed.
            
## After Approval
Once an RFP is approved, the submission period will start. The RFP manager will create a post on the DAO forum 
for proposals. 

After the submission period is completed, the manager will select a winning proposal. Normally, the manager will 
be one of the stewards of the working group who has adopted your RFP.

## Executable Proposal
If your proposal is an Executable Proposal, you will now need to submit it to the governor contract for voting onchain.

To enact an Executable Proposal:
1. Ensure at least 100k ENS is delegated to your address in order to submit a proposal, or find a delegate who has 
   enough delegated ENS to meet the proposal threshold to propose on your behalf.
2. Call the propose() function of the ENS governor (at [governor.ensdao.eth](https://etherscan.io/address/0x323a76393544d5ecca80cd6ef2a560c6a395b7e3)) 
   to deploy your proposal.

Once the propose() function has been called, a seven day voting period is started. Ongoing discussion can take place 
on your proposal post. If the proposal passes successfully, a two day timelock will follow before the proposed code 
is executed.

## Begin Work        
The person who wrote the proposal, can then start the work. They get paid for meeting RFP milestones and 
progress specified in their proposal. The RFP manager approves these requests and allocates the funds from 
the budget.


    


---
## Footer
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

## Best ENS VIDEOS 

### ENS Sessions
- Session 1: DNS Integration - https://www.youtube.com/watch?v=wSF_f3cJpy8
- Session2: Governance - https://www.youtube.com/watch?v=sGej7AbD_EY
- Session3: Layer 2 - https://www.youtube.com/watch?v=9DdL7AQgXTM
- Session4: Show & Tell - https://www.youtube.com/watch?v=tZWRO6srhZw


### ENS Workshops
- ENS Workshop 1: ENS as NFT v2 (aka Name Wrapper) - https://www.youtube.com/watch?v=MRiBdqE3pDc
- ENS Workshop 2: ENS name as web3 profile - https://www.youtube.com/watch?v=Eiq1m2iNK6I


### References
https://discuss.ens.domains/t/second-draft-of-the-ens-dao-by-laws-for-comment/11462

### Working Groups
https://discuss.ens.domains/t/ep12-social-working-group-rules/12953

https://discuss.ens.domains/t/ep14-social-dissolve-community-working-group/12982

https://discuss.ens.domains/t/ens-dao-town-hall/12751/17

https://www.figma.com/file/Acprf74LL8mfRAehfyQZir/ENS---Podarchy-(alisha.eth)?node-id=0%3A1

### Steward
https://discuss.ens.domains/t/how-it-will-work-steward-nominations/9212

https://discuss.ens.domains/t/steward-election-q3-q4-2022/13185

### ENS Dashboard
https://datastudio.google.com/u/0/reporting/8785928a-71d5-4b17-9fea-fe1c937b064f/page/RoKgC

ENS Constitution
https://discuss.ens.domains/t/proposed-ens-constitution/814
https://ensdao.eth.limo/constitution.pdf  (First Four Pages)
https://docs.ens.domains/v/governance/ens-dao-constitution

Proposal Process
https://docs.ens.domains/v/governance/process#the-rfp-process


    
