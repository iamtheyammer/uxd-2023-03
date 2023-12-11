---
layout: single
title:  "Usability Testing Results"
date:   2023-12-11 11:44:00 -0400
permalink: /phase-3/usability-testing-results
categories: phase-3
excerpt: "Here's what our users said about our prototype!"
---
## General Overview

We tested our Figma prototype with four older adult users, most of whom we had talked to in earlier phases. Overall, the reaction was very positive, and multiple users said they wish our product existed. Based on what we knew about how our users interact with software, we designed redundancy into our application by displaying written instructions and highlighting the area on the screen to click. Users relied on both to figure out what to do. All users were able to complete the tasks of adding and manipulating passwords on a user-hostile password manager website, despite some of them having never used a password manager (and none having seen that specific website) before.

## Experiment (A/B Test) Results

After testing with four users, we learned that the taskbar launch option is the most intuitive for our users and the best way to move forward. Although users remembered how to open the sidebar with both options, the taskbar option was opened faster in the initial step, and preferred by our users when asked. The taskbar option is how they “open up other computer programs anyway” and they didn’t see any reason “to reinvent the wheel”. Specifically, the wording “want help?” came directly from a user whom we had talked to before, so it was especially intuitive for that user.

We believe if we completed the full user study with 10 older adults, we’d likely see comparable results. One of the reasons we chose the taskbar option as a variant in our A/B testing was for the aforementioned reasons our users cited. This goes back to one of our original insights in phase 1 where we wanted to minimize reliance on technological touchstones that our user group does not necessarily have. By removing assumptions about the user’s application knowledge, we cater to older adults.

## Going Forward

One thing we realized across multiple tests is that we describe the color of buttons (ie “press the red button”) when they are highlighted. Since the highlight changes the color, this is not clear. We should fix this by changing our descriptions of these buttons.

We also discovered that having the last step remain highlighted after it has been completed causes confusion since it is not consistent with how the rest of the steps become darker after completion. We should fix this by un-highlighting the last step on the completion screen.

Some users had trouble finding the highlighted area on the screen. We should experiment with adding animation to draw attention to the highlighted area. The animation should occur when the instruction first appears, and there should be a way for the user to replay the animation. One idea is to have a button that says “show me where to click,” and another idea is to replay the animation when the user clicks on the active step in the sidebar.
