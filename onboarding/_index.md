---
title : "2.Account Onboarding"
description : "Attest Project Plan and Roadmap"
---

## Attest Overview and Interactive Demo Presentations




{{% notice tip %}}
Download latest Netspective Attest Overview
{{% /notice %}}

{{% button href="./_index.files/Netspective Attest Overview.pptx" icon="fa fa-download" %}}Tour Document{{% /button %}}



{{% notice tip %}}
Download latest Interactive Demo Document
{{% /notice %}}

For trying out use Attest Training environment


{{% button href="./_index.files/Netspective Attest Interactive Demo.pptx" icon="fa fa-download" %}}Interactive Demo Document{{% /button %}}

{{% button href="https://training.attest.cloud" icon="fa fa-download" %}}Go to Training Site{{% /button %}}


## Attest User Onboarding Flow



{{<mermaid>}}
sequenceDiagram
    
    participant U as EndUser 
    Participant W as Attest.cloud
    Participant CRM as CRM Tool
    Participant MU as GrowthHacking Team 
    Participant A as Attest
    Participant R as Analyst

    U->>W: Landing Page
    U->>W: Demo Request with email,contact details to User Onbording Campaign
    W->>U: Thank you for interest mail

    W -->> CRM :Added Lead to CRM as Entry
    CRM-->>MU : View the lead Entries
    MU->>U: Follow up the Demo Request
    CRM-->>MU : Verify the lead Entries
    MU->>A: Create Demo Account and Assessment for User
    Note left of A: Use predefined demo assessment questionnaire and create an account and user to do demo assessment
    A->>U : Send Account Welcome Email with Assessment Request
    MU->>CRM : Initiate Follow Up with Demo Assessment Request
    loop reminder
        MU->>U: Demo request reminder
        A ->>U: Assessment request reminder
    end
    A->>U : Send reminder for Demo Assessment if EndUser didn't start Assessment
   U->>A :Login to Attest 
   alt is Assessment Not Started
        MU->>U: Demo request reminder
        A ->>U: Assessment request reminder
   else Save Assessment
       MU->>U: Demo request reminder for complete 
        A ->>U: Assessment request reminder for complete 
     
    end
    opt Complete Assessment
        U->>A : Complete the demo Assessment
    end
 
    A-->>A : Generate calculated score for the demo assessment
    A->>U: Send demo assessment completed notification
    R->> A: Reviewer review the demo assessment with review score and comments
   MU->>U: Follow up the Demo Request

{{</mermaid>}}

## Onboarding Documents

{{%attachments style="blue" /%}}


