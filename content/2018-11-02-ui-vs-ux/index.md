+++
title = "UI vs. UX in-depth: Why you need to know the difference"
date = 2018-11-02T20:53:02.263Z
draft = false
description = "A guide to everything you need to know about UI and UX design, with easy-to-follow examples."

[taxonomies]
authors = ["Alexander Lozada"]
categories = ["design"]

[extra]
cover = "cover.png"
+++
**If you're looking to become a better designer, or want to know what makes some apps great, understanding UI & UX in depth is essential.**  

While both fields relate, individual practice and thought are still necessary.

# What is design?

Before we get into how UI & UX differ, it's important to have a grasp on the definition of design.  Most folks say that design “makes things look pretty”.  My definition is a bit more all-encompassing.

Design is everything.  I know that answer is a cop-out, but stay with me.  Design is any structure that conveys meaning or purpose to a user.  Websites have design, furniture has design, software has design, and even [languages have design](https://en.wikipedia.org/wiki/Lojban).

In this story, we're concerned *mostly* with **visual design**.  Visual design explores human sight, perception, and psychology.  Product design, web design, graphic design, and interior design are all examples of visual design.  As it so happens, UI & UX are on that list, too.

{{ gifv(path="arrowspin") }}

## What is UI and UX Design?

User interface (UI) design includes topics like colors, typography, and spacing.  This is the “pretty” part.

User experience (UX) design is the way our product functions.  UX helps us guide users in various tasks such as signing up for a newsletter or navigating to a specific page.  It is more about how something *functions* instead of how something *looks*.

Today, we're focusing on the most common applications of UI/UX design.  This includes desktop applications or websites.  However, UI/UX isn't limited to this space and has applications in many diverse fields.

# In-depth: User Interface

User interface (UI) design is the application of design rules to interactive or informational elements.  It defines how interfaces look through usage of colors, spacing, typography, and more.  There are a few key reasons why UI design is so important:

## It helps users know where to look first

Newspapers contain a ton of words, images, and advertisements.  Yet readers still navigate them with ease.  How is that possible?  Consider the following examples.  Which is easier to parse?
{{ image(path="comparison.png", description="Small changes can make a huge difference.", alt="A split image of text.  The right side is more organized due to hierarchy.") }}

You likely chose the second image, but why is that?  Limited to text elements, font size groups content into easier chunks.  This is an aspect of **hierarchy**.  Hierarchy in design dictates what viewers see first.

Hierarchy is not limited to sizing.  It involves anything that makes an element stand out.  We can use color, spacing, and font to denote hierarchical elements.

{{ image(path="hierarchy-none.png", description="With no hierarchy, all elements appear to have equal importance.", alt="An example of a layout without hierarchy") }}

{{ image(path="hierarchy-color.png", description="A different color can draw attention and establish hierarchy.", no_top_margin=true, alt="Using color to show hierarchy") }}

{{ image(path="hierarchy-size.png", description="Size has a similar effect.", no_top_margin=true, alt="Using size to show hierarchy") }}

Hierarchy is present everywhere — not only print media.  This site uses *spacing*, *font*, and *sizes* to split up elements.  

## It helps users understand what to tap or click

Whenever you use an app on your phone, you're making decisions. “Should I make this post public? Should I get the 2-day shipping? Should I comment on this website?”  Visual design gives cues on what decisions to make, and how to interact with interfaces.

Imagine you're creating a website, and you want to link to your friend's blog.  How should that link look?  You use plain text that says “Look at this blog!” in your first iteration.

{{ image(path="affordances.png", alt="Buttons are UI elements with affordances") }}

This isn't working, but why?  It's because users expect interactive elements to share specific visual aspects.  In your case, a simple underline will denote a hyperlink.  These expectations are examples of [affordances](https://en.wikipedia.org/wiki/Affordance) (which also deserve their own story).

{{ image(path="affordances-b.png", alt="A simple underline shows that this is a link.") }}

Buttons are rectangles with text.  Links have underlines.  Text inputs have labels.  Applying expected visual styles to interfaces allows us to show behavior without explanation.  This doesn't mean we can't experiment.  But having structure helps us to build unique interfaces with clarity.

There is much, much more to UI design, and it deserves its own story.  These examples mean to give an idea of UI's importance.

{{ image(path="link.png", description="We expect certain UI elements and interactions when using a digital device.", alt="A retro style scene with a computer monitor and application window") }}

# In-depth: User Experience

User experience (UX) design focuses on how users interact with something.  Think of UX as creating a story-line for users to follow.  When designing an application with UX in mind, user goals must be considered.

For instance, assume you are designing a web store, and you want to guide a user through checkouts.  You want the *flow* of those interactions to be as easy as possible so that nobody gets frustrated.  You would make the user go through logical pages and clicks.

{{ image(path="user-journey.png", description="You could even shorten this process and add a simple “buy now” button like Amazon.", alt="A simple example of a text-based user journey") }}

This is a very simple example of a **user journeys**.  User journeys illustrate what steps users go through to accomplish a task, and are a fundamental aspect of UX design.  Note that the journey didn't need to include anything but text.  That's because UI covers visual design, while UX covers the base interactions.  This is a simplification, but it generally holds true.  Okay — I know I said UX is part of visual design, and that's true for app and web design.  However, the concepts of UX apply almost everywhere!

A simple text-only app can benefit from UX considerations.  Everything from text adventures to code compilers design with user experience in mind.  

First, lets pretend we're creating a text adventure.  

```
> You enter a room.  It's dark.
```

We want the player to type “turn on lights”.  However, not every player will think this way!  This is what happens when our play tester enters something invalid.

```
> You enter a room.  It's dark.

RESPONSE: use my phone flashlight

> Hmm, that doesn't seem to work.  Try again.
```

This response from our text adventure is vague and unhelpful!  It gives our players no feedback, and it may even annoy them.  Let's use UX to solve this problem.  Our goal is to get the player to turn on the lights.  Our player's goal is to find the right command.  Instead of giving back a vague response, we can format some help items!  Here's what that might look like.

```
> You enter a room.  It's dark.

RESPONSE: use my phone flashlight

> Hmm, that didn't work.  I understand the commands LOOK | TURN ON | OPEN | USE
```

Now our player has a base understanding of what commands *will* yield a response.  The same is true for UX design in any medium!  It's all about the user's path, choices, guidance, and experience.

## For programmers

If you're coming from a development background, there are great examples of UX in applications and toolchains.  For example, The [Elm language compiler](http://elm-lang.org/) (a program that converts programming languages into computer code) is an example of a program out in the wild with great UX.  Its main purpose is to help programmers fix mistakes in their code, and it does so with hints.  Solving a user problem through hints, and guiding them to a correct path is an example of great UX.  The Elm compiler gives users a hint on how to fix their code at the bottom.

```elm
-- TYPE MISMATCH ---------------------------- Main.elm

The 1st argument to `drop` is not what I expect:

8|   List.drop (String.toInt userInput) [1,2,3,4,5,6]
               ^^^^^^^^^^^^^^^^^^^^^^
This `toInt` call produces:
    Maybe Int  
But `drop` needs the 1st argument to be:
    Int  
Hint: Use Maybe.withDefault to handle possible errors.
```

# Ideas used in UX design (with examples)

User experience design involves numerous processes.  Here we'll highlight a few.

## Personas

Think of personas as potential users.  For instance, if you're making a banking app, you could have personas like these:

| Name      | Persona                                                                                                                                                                                                                                   |
| :-------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Maria     | She's 18 and looking for a way to keep track of her finances.  She still lives with her parent, and doesn't have a job.  She wants a way to check that she has enough money to go out with friends, and make sure she isn't overspending. |
| Johnathan | He's 46 and married with 2 children.  He is paying off a house and has trouble remembering to pay his mortgage on time.                                                                                                                   |
| Jules     | They're 24 and single with a full-time job.  They're saving up for a house and need help keeping track of expenses.                                                                                                                       |

All three users are using the same application, but have different goals.  Maria might want a spending tracking feature.  Johnathan might want an auto-pay feature.  Jules might want a gamified savings account.  

Personas help us design around **user goals**.  They are a part of [user-centered](https://en.wikipedia.org/wiki/User-centered_design) design, which is an essential part of UX.

# Summary: UI vs. UX

Let's recount what we learned:

## UI Design

- Based around visuals like color, shape, and typography
- Establishes hierarchy which breaks information into digestible chunks
- Helps denote which elements are interactive, and how they will behave

## UX Design

- Based around more abstract user flows
- Helps the user achieve their goals
- Can be non-visual 

# Where UI and UX Overlap

UI and UX are separate concepts that make up a whole.  Many times, they can blur together.  The visual aspects of user interface can *guide* the user in a specific experience.  A user experience can *guide* the user to see certain visual elements.

Imagine you have a web store again.  You have an “Add to cart” button, as well as a “See related items” button.  Your goal is to get a user to buy something first, and see related items second.  The user's goal is to easily browse and use our store.

You can guide the user via UI design into your desired path.  We can make the “Add to cart” button more visible and thus more likely seen.

{{ image(path="ui-ux-overlap.png", description="UI and UX can work together to help the user select options easily.", alt="Comparing different versions of sites with alternate UI and UX") }}

Note that "Big and colorful" does not always mean users will happily click through, especially when other UI elements are at play.

# Conclusion: Why is the difference important?

**User experience is like a foundation, and user interface is like a house.  You can build a pretty house, but with no foundation it will crumble.  You can lay a solid foundation, but it will be uninhabitable without walls and a roof.**  If you don't know the difference, then you can't use the tools specific to each one.  Having a solid grasp of the differences help build a path towards improving your work.

## How can I improve?

UI and UX work together.  When designing, keep basic principles in mind.

**User Experience**: Remember these points for a seamless experience.

- Design around the user
- Solve the user's goals
- Create personas to cover all use-cases
- Create a framework or wireframes to illustrate a user's journey

**User Interface**: Keep the following in mind to make your designs shine.

- Utilize hierarchy to highlight and group
- Use color, spacing, and typography in a way that helps your users achieve their goals
- Reinforce your UX design with beautiful but logical visual choices

# A question for you

Did you find this story helpful?  If you did, share it and help someone else.  You can also subscribe to our design newsletter soon!

In the comments below, I want to know how you plan to use UI & UX in your next project.
