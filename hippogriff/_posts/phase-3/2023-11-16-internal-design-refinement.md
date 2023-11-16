---
layout: single
title:  "Internal Design Refinement"
date:   2023-11-16 11:01:00 -0400
permalink: /phase-3/internal-design-refinement
categories: phase-3
excerpt: "We've decided on a feature to implement. Now we need to figure out how to make it work."
---

## Design Phase Introduction

The first half of this phase of the project consisted of rendering our paper prototype into Figma. Once we had a full interactive user flow with multiple paths, we worked with our peers to gather feedback based on Jacobson's usability heuristics.

## Changes from Paper Prototype to Figma

Paper is a much looser format that allows users to make key decisions about the big picture items of a prototype. Some of these critical themes we saw were:

* The major component of the app (all the cheat sheets) should be a sidebar and not a floating box. If it pops up in front of the screen, it may block visibility of the very thing the user is requesting help with. This would have been a huge set back had we realized this later than the paper phase. A sidebar is also usually assumed to be a vertical format, which gives users automatic information on how to use it.
* Search bar should be at the top of the sidebar, and always visible. Our user group lacks technological context, so relating to any previous experience they have is critical. In some of the most common websites older adults use (Google, Streaming Services, ect), the search bar is always at the top. Additionally, elements that move should have a reason for doing so, there’s no reason for the search bar to ever disappear, because a vertical format gives us plenty of screen real estate for horizontal items.
* Tooltips are necessary along with detailed instructions, pictures and visual aid is key. If you’ve never used some feature before, It’s easier to visually match that two icons look the same than match the name of some button (Bold button) to some arbitrary icon (Capital B icon).
* It’s important to be able to see all instructions in order and have the option of going back to a previous step. Empowering users to take control of their own experience with an app is important in making software feel intuitive. You should design such that users only ever want to use your app in the intended way. If they have an urge to do something within the interaction of your app and can’t, then it’s an inherently frustrating feeling.

Moving to figma comes with a level of polish and scalable interactivity that are helpful when evaluating an interface. It also adds the automation that is characteristic of software apps and not necessarily of physical mediums like paper. Here are some major elements we included to realize our prototype in figma:

* Icons should be clearly clickable or not clickable when representing a potential action vs quick visual aid. Users may unintentionally click something that they may believe to be a button when it’s just an informative icon. This either leads to nothing happening, or a user getting dragged into an action they didn’t want to do. Either way, it’s confusing and may reinforce bad usability habits.
* Boundaries between different sections and actions need to be clear and consistent. Stuff needs to be organized in a way that makes it obvious what information goes with what sections/actions/tabs etc.
* Wording should be designed with older adults in mind. We should avoid technical terms like PDF where possible.Wording should be designed with older adults in mind. We should avoid technical terms like PDF where possible
* Cursor interaction is an important tool for 1st Nielsen Heuristic, seeing the cursor change is not a feature of figma and made us think more intentionally about how to design our product in a clear and concise way. Without the ability to indicate something’s a textbox (“I” shaped cursor), or that something’s clickable (hand with pointer cursor), relating to users’ previous technological touchstones becomes incredibly important.
* We also need to think about what other applications will pop up when a user performs an action, such as a file manager window when someone saves a PDF. Our software should anticipate these extra steps and include them in the step-by-step list without extra button clicks.

However, one of the big challenges when moving to Figma is determining what should be interactable (what can be clicked and what’s there for looks only). Since we’re using a screenshot of Google Docs and building on top of that, there are a ton of buttons that appear clickable, but, since those buttons aren’t applicable to our app’s mission, we didn’t make them interactable.

On paper, this isn't a thought. It’s clear what’s interactable and what’s not based on the physical pieces of paper. However, on Figma, most users don’t know that they can click out of the window to see blue outlines on interactable objects. To bridge this gap, we decided to make things in Google Docs that can be clicked highlighted in green. This way, it’s clear which Google Docs icons can be clicked and what can’t.

## Explanation of our Prototype

Our Figma prototype doesn’t vary too wildly from our paper model. Again, we used Google Docs as an example of software that a user may need help with. 

In the bottom right corner there’s a help button that activates our app in a sidebar. This sidebar has a search bar at the top with buttons for suggested quick actions below. Once a user searches for and/ or selects what they are trying to accomplish, the sidebar is replaced with step-by-step instructions and corresponding tooltips appear on screen. 

We experimented with two different aesthetic implementations for this instruction/ tooltip flow so that we could compare our feedback for both. 

See an interactive demo of our initial Figma prototype below. Draft interactions have been implemented for saving a PDF and creating a numbered list. As noted before, each interaction flow is intentionally different.

Note: The prototype shows up pretty small! We recommend pressing the full-screen button that appears at the top right of the embedded frame.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FogBoDqiZhpJV8jtunDc7tw%2FPrototype-1-(Google-Doc)%3Ftype%3Ddesign%26node-id%3D5-6%26t%3DdjddHjTFWwbmpes8-1%26scaling%3Dscale-to-fit%26page-id%3D0%253A1%26starting-point-node-id%3D5%253A6%26mode%3Ddesign" allowfullscreen></iframe>

## Internal Feedback

Following the creation of our prototype, we engaged with Team Wendigo, another group in our class, to test our design and gather feedback. Their insights proved valuable, highlighting key areas for cosmetic and usability enhancements in our product.

### Cosmetic Feedback

One of the primary challenges our team identified was the integration of our product within the website the user is navigating. The reviewing team had difficulty distinguishing between our product's interface and the sample Google Docs environment. This observation underscores the importance of color selection in enhancing user experience and interface recognition. To address this, we will explore a more dynamic use of color. Selecting hues that contrast effectively with various websites will be crucial. This will ensure our product stands out and is easily identifiable, regardless of the background interface. Additionally, we currently use yellow to highlight the focused element. However, we are considering a more dramatic approach, such as dimming the entire screen except for the focused element. This could provide a clearer visual cue for users and further improve visual contrast for our design.

Another feature that may need to be altered cosmetically in the future is the help feature, marked by a question mark. It is currently positioned in the bottom right corner and can be easily overlooked, and we noticed many of Team Wendigo’s members struggled to identify where to click to find our product. We plan to edit this feature and possibly position it to a more prominent location and redesign its icon for better visibility and accessibility.

More generally, Team Wendigo noted that our sidebar may be overwhelming considering how much content is already on screen. They advised we should include minimal information at any given time to prevent overcrowding.

### Usability Feedback

On the usability side of things, a significant portion of the feedback we received centers around the application's use of technical terminology, which can be challenging for our primary user group, older adults. To make our application more accessible and user-friendly, we plan to introduce visual aids and simple definitions alongside complex terms, such as 'PDF' or 'drop-down'. This will help demystify technical language, making it easier for users to understand and interact with the application. Additionally, we aim to educate our users about common computer symbols. Instead of just showing pictures of buttons, we will provide their names, helping older adults to familiarize themselves with these symbols and enhance their computer literacy.

Another crucial area of improvement is in the application's response to user errors. We currently don’t have any signifiers in place to inform users if they made a mistake or are going off-track from the task they are trying to achieve. From Team Wendigo’s feedback, we recognized the importance of providing constructive feedback without causing frustration or confusion. To achieve this, we will look for ways to implement polite and clear error messages that not only notify users of their mistakes but also guide them back on the correct path. This approach is designed to create a supportive and encouraging user experience, reducing the likelihood of users feeling overwhelmed or lost.

### Feature-specific Feedback

Feedback on specific features of the application has also highlighted areas for enhancement. One key point is the potential information overload caused by a scroll bar, which can be overwhelming for older adults trying to navigate the platform. Looking ahead, we will focus on the search bar, making it the most prominent feature. This decision is based on the understanding that a straightforward and accessible search function is more suitable for older adults, as it simplifies navigation and reduces complexity.

Additionally, we noted that the lightning bolt symbols on various options were not perceived as clickable elements but rather as static icons. To make these interactive elements more intuitive, we will look at ways to replace the lightning bolt symbols with descriptive text like “Do It For Me.” The changes we make will need to clarify the function of this button, making it more user-friendly and reducing ambiguity about its purpose. By making these adjustments, we aim to create a more intuitive and user-centric application, specifically tailored to the needs and preferences of older adults.

## Moving Forward

Moving into our external review phase, we want to know if we have simplified our design enough that it is intuitive for older adults. In this phase, we forewent user feedback from older adults in favor of heuristic assessment from our fellow designers in the class. In the final phase, we would like to check the heuristics against our real user group.

Another small question which will benefit from user feedback is the location of the button that starts our software. We considered several manifestations of this button, including a fixed circle in the bottom right corner which we used in our Figma prototype; a floating button which can be moved around in case it blocks screen content; a task bar icon; or a physical button on the keyboard. This is how users will initially access our software, so it is critical that it be easy to find in order for our entire application to reach its accessibility goals.

## Appendix

### Effort Chart

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2Fey0GlzaAqqNzMDNqNjkAWv%2FUntitled%3Ftype%3Dwhiteboard%26node-id%3D0%253A1%26t%3DFJcq1hRWrrsbjdWt-1" allowfullscreen></iframe>

### Feedback Received

| Heuristic | Severity | Number of People | Feedback |
|-----------|----------|------------------|----------|
| H3: User control and freedom | 3 | 3 | Difficulty with the tiny 'x' on the pop-up, suggesting a clearer "emergency exit." |
| H3: User control and freedom | 3 | 3 | Inability to exit out of web worker during certain tasks. |
| H3: User control and freedom | 2 | 1 | Clicking the X button from the Fast Mode boxes closes the entire Web Worker. |
| H2: Match between system and the real world | 1 | 1 | Terms like PDF, numbered list, or new tab can be confusing for older people. |
| H2: Match between system and the real world | 2 | 2 | Confusion regarding the search tool and clickable icons. |
| H4: Consistency and standards | 2 | 2 | Confusion between the “go back” and “X” buttons. |
| H4: Consistency and standards | 0 | 1 | Positive feedback on the button highlighted in yellow as a guide popup. |
| H4: Consistency and standards | 1 | 1 | Cosmetic issue with the search bar shifting positions. |
| H4: Consistency and standards | 2 | 1 | Difficulty reading blue text on white background. |
| H4: Consistency and standards | 1 | 1 | Typo error in the Number list steps page title. |
| H4: Consistency and standards | 0 | 1 | Different descriptions for the same process in different sections. |
| H5: Error prevention | 4 | 1 | Design confusion in the numbered list task, highlighting incorrect elements. |
| H6: Recognition rather than recall | 2 | 1 | Suggestion to add a feature for reviewing instructions post-task completion. |
| H7: Flexibility and efficiency of use | 3 | 2 | Hidden fast mode shortcuts and unclear lightning bolt icon. |
| H7: Flexibility and efficiency of use | 1 | 1 | Lack of customizable shortcuts or menu arrangements. |
| H7: Flexibility and efficiency of use | 4 | 1 | Small, hard-to-locate question mark for help on the main page. |
| H8: Aesthetic and minimalist design | 2 | 1 | Overwhelming amount of options on the landing page. |
| H8: Aesthetic and minimalist design | 1 | 2 | Suggestion to use colors more effectively for clarity. |
| H8: Aesthetic and minimalist design | 2 | 1 | Redundancy of the scroll bar due to the search bar. |
| H8: Aesthetic and minimalist design | 0 | 1 | Confetti icon post-task completion seen as distracting. |
| H9: Help users recognize, diagnose, and recover from errors | 3 | 2 | Lack of guidance for error correction during task walkthroughs. |
| H10: Help and documentation | 4 | 1 | Inaccessibility of help documentation within the application. |
| H10: Help and documentation | 2/3 | 1 | Suggestion to explain the purpose of button clicks in instructions. |
