---
version: v..
key: 
id: 
slug: 
weight: 

---
 VISUAL LANGUAGE  
 FOR MEDIA CREATION

 VERSION 1.2

 Contents

[1 Introduction 4](#post-2342-%5FToc90453895) 

[2 The Ontology Behind the Visual Language 5](#post-2342-%5FToc90453896) 

[3 Primary Use Cases 7](#post-2342-%5FToc90453897) 

[4 Key Workflow Components 8](#post-2342-%5FToc90453898) 

[4.1 Assets 9](#post-2342-%5FToc90453899) 

[4.2 Tasks 11](#post-2342-%5FToc90453900) 

[4.3 Participants 13](#post-2342-%5FToc90453901) 

[4.4 Contexts 15](#post-2342-%5FToc90453902) 

[4.5 Infrastructure 18](#post-2342-%5FToc90453903) 

[4.6 Thing Shape 23](#post-2342-%5FToc90453904) 

[4.7 N Shapes 23](#post-2342-%5FToc90453905) 

[5 The Meaning of Lines 25](#post-2342-%5FToc90453906) 

[5.2 Flow 26](#post-2342-%5FToc90453907) 

[5.3 Messages 30](#post-2342-%5FToc90453908) 

[5.4 Data movement 31](#post-2342-%5FToc90453909) 

[5.5 API Calls 32](#post-2342-%5FToc90453910) 

[5.6 Data Communications Links 32](#post-2342-%5FToc90453911) 

[5.7 Associations 33](#post-2342-%5FToc90453912) 

[5.8 Example uses of lines 36](#post-2342-%5FToc90453913) 

[6 Drawing constructs and annotations 37](#post-2342-%5FToc90453914) 

[6.1 Annotations 37](#post-2342-%5FToc90453915) 

[6.2 Keys and Titles 37](#post-2342-%5FToc90453916) 

[6.3 Expanded Views 37](#post-2342-%5FToc90453917) 

[Appendix A Labels 39](#post-2342-%5FToc90453918) 

[A.1 Asset Labels 39](#post-2342-%5FToc90453919) 

[A.2 Task Labels 40](#post-2342-%5FToc90453920) 

[A.3 Participant Labels 40](#post-2342-%5FToc90453921) 

[A.4 Context Labels 43](#post-2342-%5FToc90453922) 

[A.5 Infrastructure Labels 46](#post-2342-%5FToc90453923) 

[Appendix B Best Practices 49](#post-2342-%5FToc90453924) 

[B.1 Layout Practices 49](#post-2342-%5FToc90453925) 

[B.2 Using Fixed Canvas Sizes 50](#post-2342-%5FToc90453926) 

[B.3 Shape Sizes 50](#post-2342-%5FToc90453927) 

[B.4 Icon Sizes 54](#post-2342-%5FToc90453928) 

[B.5 Showing Context in a Workflow 56](#post-2342-%5FToc90453929) 

[B.6 Creating Custom Themes or Diagrams 57](#post-2342-%5FToc90453930) 

[Appendix C Visual Language Depiction of Ontology Relationships 60](#post-2342-%5FToc90453931) 

[Appendix D Visual Language Summary 62](#post-2342-%5FToc90453932) 

 This document is intended as a guide for companies developing or implementing products, solutions, or services for the future of media creation. No effort is made by Motion Picture Laboratories, Inc. to obligate any market participant to adhere to the recommendations in this document. Whether to adopt these recommendations in whole or in part is left to the discretion of individual market participants, using independent business judgment. Each MovieLabs member company shall decide independently the extent to which it will utilize, or require adherence to, these recommendations. All questions on member company adoption or implementation must be directed independently to each member company.

 © 2021 Motion Picture Laboratories, Inc.

 This document is licensed under the Creative Commons Attribution 4.0 International License. 

 Additional Permissions (CC+): We recognize that it may be impractical to provide attribution in connection with each individual use of the iconography and shapes in this document. As such, we are hereby waiving the attribution requirements of the Creative Commons Attribution 4.0 International License solely with respect to any uses of this iconography. We will not be requiring attribution for such uses, although we would welcome attribution when reasonably possible.

 Except as specifically stated above, all of the terms and conditions of the Creative Commons Attribution 4.0 International License will apply to any sharing, reproduction, or other use of this document.

 Creative Commons Attribution 4.0 International License (CC BY 4.0) – Summary

 You are generally free to copy and redistribute the material in any medium or format, and remix, transform, and build upon the material for any purpose, even commercially, under the following conditions: 

 Attribution: You must give appropriate credit to MovieLabs, provide a link to the license, and indicate if you made changes to the material. You may do so in any reasonable manner, but not in any way that suggests that MovieLabs endorses you or your use of the materials. 

 No Additional Restrictions: You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits. 

 Note: The above text is a human-readable summary of (and not a substitute for) the license, which can be found at: <http://creativecommons.org/licenses/by/4.0/>.

# Introduction

 Humans, especially creative ones, are a visual species. We digest complex and nuanced information by drawing it out. Diagramming out complex ideas can help us see the subtleties, the interconnections between elements and where risks are and when resources should be applied. In video content creation the diagrams can be myriad – some people draw out sequential workflow tasks, some draw out which assets move through a process, some focus on the people and what they are doing in a workflow, some show the infrastructure or tools that are used at each step. Some visuals include a combination of all the above. 

 At MovieLabs we have drawn many of these diagrams, and we’ve exchanged many of them; with our studio partners and others in the industry, and we began to notice one obvious thing – none of the diagrams are the same. Sometimes they vary wildly. Different people, often within the same organization or team, draw different workflow diagrams. Sometimes there are differences within the same diagram with inconsistent approaches to conveying tasks, participants, or assets. While we have no intention of “standardizing” diagrams – because there’s no standard for expressing ideas – we do want to provide a common language that everyone in the industry can use to express their ideas. A language defines concepts and grammar but of course still leaves the user to express their ideas however they want. That, and an underlying data structure across connected ontologies, is what let us to create the MovieLabs Visual Language for Media Creation (VLMC, or Visual Language).

 The Visual Language is intended to be used by those drawing out workflow diagrams, those trying to convey a particular idea or production concept and those creating software or tools to make it easier to create, view and modify those workflows. The Visual Language was intended for Human-to-Human communication, but we also foresee use cases where it can be used for Machine-to-Human Communication (for example a status dashboard showing tasks working through a software defined workflow) or Human-to-Machine Communication (for example drawing out workflows which are then used to program an automated software defined workflow)

 There are three key components in the Visual Language package:

**Definition and Guide:** This document describes the various shapes, labels, and icons as well as the lines and arrowheads used to connect shapes in the language. This document also describes the best practices and the connection between the Visual Language and the common Ontology.

**Resources:** This is a set of resources to use the language including icons, shapes, and libraries (with common file formats like SVG and PNG assets).

**Templates:** The final package is a set of templates in various diagramming or presentation tools. The current templates are in LucidChart, PowerPoint and Visio. 

# The Ontology Behind the Visual Language

 The elements depicted in the Visual Language are supported by the MovieLabs Ontology for Media Creation (OMC),[\[1\]](#post-2342-footnote-2) which we developed for improving communication, interoperability, and automation of production workflows as part of the MovieLabs 2030 Vision project.[\[2\]](#post-2342-footnote-3) The ontology groups workflow elements into general categories including tasks, assets, participants (e.g., organizations, departments, people), contexts (e.g., scenes, shots), infrastructure, and the relationships between them. It also provides some more detailed categories (e.g., image vs. audiovisual assets) and defined terms for many more specific elements.![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-128.png) 

 Figure ‑ Ontology for Media Creation

 In some cases, these categories and defined elements are important enough to have specific depictions in the Visual Language as shapes or icons. In other cases, the names and terms can be used as labels.

 Like the use of common shapes and icons, the use of common labels makes it easier to understand what a diagram is trying to illustrate. And the definitions behind the terms give diagrams greater precision. These labels are listed in Appendix A.

 In its initial release, the Ontology covers around 200 of the many thousands of elements in production workflows. When an element in a diagram needs a label, we encourage the use of the common term from the Ontology, if the definition fits and provides the necessary level of specificity. But in many cases, users of the Visual Language will need to create their own names for things. Future releases of the Ontology will expand the coverage still further.

 It’s also worth noting that elements can fall into more than one category. For example, a prop can be regarded as an asset or used as a context for a task. And an automated service can be regarded as a participant performing a task or as infrastructure. So, the shape that is used for an element may vary based on what is being communicated and the message that the creator wants to show. The details of how this works can be found in the ontology documentation. 

 The Ontology also defines relationships between elements that can be depicted in the Visual Language, often using lines to connect those elements. For those implementing the Visual Language in software that uses the Ontology, Appendix C describes the visual depiction of relationships in the Ontology.

# Primary Use Cases

 The primary use cases for the Visual Language are for the visual communication of information about content creation workflows, whether between people, between machines, or from machines to people. 

 They include: 

* Building and configuring a pipeline / integrating tasks and infrastructure
* Designing workflows (high level) comprised of assets, tasks, and participants  
   * Understanding asset/data flows between set, clouds, on-prem, vendors, participants  
   * Ensuring input/output compatibility across boundaries (formats, color practices, etc.)
* Workflow status dashboards and reporting tools

 The following is a workflow diagram for a finishing process which we will use as an example:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-129.png) 

 Figure ‑ Finishing Workflow

# Key Workflow Components

 The first order of the Visual Language is to represent the five key categories of workflow components: Assets, Tasks, Participants, Infrastructure and Contexts. We will separately describe the relationships that may connect these in a workflow in the following section “The Meaning of Lines”.

 MovieLabs defines these terms as follows.

* _Context_: Informs scope within the construction process of a Creative Work.
* _Asset_: A physical or digital object or collection of objects specific to the creation of the Creative Work.
* _Participant_: The people, organizations, or services that are responsible for the production of the Creative Work.
* _Task_: A piece of work to be done and completed as a step in the production process.
* _Infrastructure:_ The underlying systems and framework required for the production of the Creative Work; it is generally not specific to a particular Creative Work.

 For each of these categories, the Visual Language provides the following:

* **Shape**: A shape that can visually differentiate it from elements in other categories.
* **Icons**: Icons that visually identify different classes of elements in the same category. The set of predefined icons will grow over time.
* **Labels**: A set of defined terms for classes of elements that can be used to label diagrams consistently.

 Users of the Visual Language must use the provided shapes, icons, and labels, unless they need to depict something more specific or otherwise not covered by the current specification. 

 The five primary shapes are shown below.

![Text

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/text-description-automatically-generated-5.png) 

 Figure ‑ The primary Visual Language shapes

 The following sections provide more detail.

## Assets

 Assets are the things that a Creative Work is made from. Storyboards, camera footage, props, and 3D Models are all examples of Assets. 

**Asset**: A physical or digital object or collection of objects specific to the creation of a Creative Work.

### Asset Shape

 The Asset shape is a square with rounded corners.

![Text

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/text-description-automatically-generated-6.png) 

 Figure ‑ Asset shape

 The aspect ratio of the Asset shape must be 1:1.

### Asset Icons

 The Visual Language icons allow for the identification the intrinsic nature of an asset, as opposed to its use. Let’s look at how we use that.

 The icon for an image is this:

![Icon

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/icon-description-automatically-generated-1.png) 

 Figure ‑ Image icon

 When the image icon is used in the asset shape to visually identify the nature of the asset, it may be necessary to add text to qualify what sort of image it is. Other icons are a composite of two primitive icons. For example, the icon for an audio-visual asset is the combination of the image icon and the audio icon.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-130.png) 

 Figure ‑ Composite icon

 The current set of asset icons are:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-131.png) 

 Figure ‑ Asset icons

 Examples of the use of these icons are:

| **Icon**        | **Examples**                                                                                    |
| --------------- | ----------------------------------------------------------------------------------------------- |
| Image           | A jpeg file – digital image. A photograph – analog image, a storyboard.                         |
| Moving Image    | Digital cinema camera files – digital moving images. 35mm film negative – analog moving images. |
| Audio           | A WAV file – digital audio. A vinyl record – analog audio.                                      |
| Audio Visual    | A ProRes file – digital audio visual. 35mm film print – analogy audio visual.                   |
| Document        | A PDF file – digital document. A piece of paper – analog document, a script.                    |
| Physical Object | Prop, Set, Costume                                                                              |
| Group           | USD, AAF, ZIP                                                                                   |

 The icons provided above should be used when the asset meets the definition, unless a more specific visual depiction is needed. Assets that are not covered by the current icon set can be depicted with the basic shape and a user-provided label or a user provided icon, or both. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-132.png) 

 Figure ‑ Three ways to show an asset when there is no appropriate icon

 In Figure 4‑6 the icon is (rather obviously) supplied by the user.

### Asset Labels

 When a specific icon is not available or more information is required, asset labels are used to further identify the type of asset. The current set of asset labels are listed in Appendix A. While not comprehensive, the set will grow over time.

### Example Use of Asset Shapes, Labels, and Icons

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-133.png) 

 Figure ‑ Example workflow with assets and asset icons emphasized

## Tasks

 Tasks are the steps or activities that are carried out in the production process. 

**Task:** A piece of work to be done and completed as a step in the production process.

### Task Shape

 The Task shape is a symmetrical trapezoid[\[3\]](#post-2342-footnote-4) on its side with rounded corners.

![Text

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/text-description-automatically-generated-7.png) 

 Figure ‑ Task shape

 The aspect ratio of the Task shape must be 4:3\. Although the Task shape is asymmetric, things going into and coming out of the task may do so on any side. However, the task shape must be used in the orientation shown in Figure 4‑8\. It must not be rotated or flipped horizontally. 

 The ability to have a shared view of a given Task across all the systems used in a production is key to the collaboration tenets of the 2030 vision.

### Task Icons

 In the first version of the Visual Language there are no icons for tasks which must be depicted using the basic task shape and a user-provided label.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-134.png) 

 Figure ‑ A set of tasks depicted using task shape and user provided labels

### Task Labels

 When a specific icon is not available or more information is required, task labels are used to further identify the type of task. The current set of task labels are listed in the appendix A. While not comprehensive, the set will grow over time.

### Example Use of Task Shapes and Labels

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-135.png) 

 Figure ‑ Example workflow with task shapes emphasized

## Participants

**Participant**: The people, organizations, or services that are responsible for the production of the Creative Work.

 People are the individuals that are contracted or employed to perform given tasks on a production. Organizations are groups of people or legal entities with a particular purpose relative to the production. Services are computer driven agents that can perform tasks given the proper context and structured data input.[\[4\]](#post-2342-footnote-5) 

### Participant Shape

 The Participant shape is a hexagon with each side the same length (that’s an aspect ratio of 1:0.87).

![Text

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/text-description-automatically-generated-8.png) 

 Figure ‑ Participant shape

 Defining Participants in a software defined workflow is crucial for automation, security, and production management. 

### Participant Icons

 The Visual Language icons allow for the identification the intrinsic nature of a participant, as opposed to its use. The current set of participant icons are:

![Shape

Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-description-automatically-generated-with-me-1.png) 

 Figure ‑ Participant Icons

 The icons provided above should be used when the participant meets the definition, unless a more specific visual depiction is needed. 

 Examples of the use of these icons are:

| **Icon**     | **Examples**                                  |
| ------------ | --------------------------------------------- |
| Person       | A director, actor, or Production Designer.    |
| Organization | Production company, VFX house, Art Department |
| Service      | Encoding, Transfer, Archive                   |

### Participant Labels

 When a specific icon is not available or more information is required, Participant labels are used to further identify the type of participant. The current set of participant labels are listed in the appendix A. While not comprehensive, the set will grow over time.

![Shape

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-description-automatically-generated-2.png) 

 Figure ‑ Example of use of participant labels

### Example Use of Participants Shapes, Icons, and Labels

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-136.png) 

 Figure ‑ Example workflow with participants emphasized

## Contexts

 Informally, we think of Context as anything that is not directly included in the set of Assets, Tasks, Participants, and Relationships needed to do a job. 

**Context:** Informs scope within the construction process of a Creative Work.

 Context is an important concept. In many circumstances, a large amount of Context can be derived from the Assets, Tasks, and Participants, but this is often a manual process (such as finding a Slate ID in video and deriving a Scene Number from it.) Context is used to aid efficient communication of important contextual information both in diagrams and in the use of the ontology. While a Context can have all sorts of other things in it, for example notes about the reasons for performing a particular Task, but there are some concepts that are globally important.

 In addition to the general Media Creation Context there two specific Contexts. Narrative Context covers the abstract concept of the who/what/where/when that together make up the narrative being created by the production. Production Context deals with the details of turning the narrative into a Creative Work. 

### Context Shape

 The Contest shape is a circle with a 1:1 aspect ratio.

![Text

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/text-description-automatically-generated-9.png) 

 Figure ‑ Context shape

 The aspect ratio of the Context shape must be 1:1. 

### Context Icons

 The Visual Language icons allow for the identification the intrinsic nature of a context, as opposed to its use. The current set of context icons are:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-137.png) 

 Figure ‑ Context icons 

 Examples of the use of these icons are:

| **Icon**           | **Examples**                                    |
| ------------------ | ----------------------------------------------- |
| Creative Work      | Moby Dick, Gone with the Wind, A Bridge Too Far |
| Character          | Dracula,                                        |
| Portrayal          | Cary Grant, Marilyn Monroe, Orson Welles        |
| Location           | Paris, Mars, Rick’s Café                        |
| Prop/Set Dressing  | Light Saber, Wallpaper, Light Switch            |
| Script             | V 1.0, Shooting Script                          |
| Slate              | Scene info (Scene, Take, Location)              |
| Slate UID          | Take 21, Scene 21                               |
| Shot               | 45, Getaway 4                                   |
| Sequence           | JRUN, 14                                        |
| Narrative Scene    | Sven meets Kiera, INT                           |
| Production Scene   | Jungle Run Crash, 12                            |
| Shoot Day          | 4, 23-7-21                                      |
| Costume            | Hat, gloves, Shirt                              |
| Storyboard         | Scene 12, Action Sequence                       |
| Reference Material | Bible, Car Manual, Wikipedia                    |
| Set                | Kitchen, bar, bedroom                           |
| Concept            | Character sketch, mood board                    |

### Context Labels

 When a specific icon is not available or more information is required, context labels are used to further identify the type of context. The current set of context labels are listed in Appendix A. While not comprehensive, the set will grow over time.

### Example Use of Context Shape, Label, and Icon

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-138.png) 

 Figure ‑ Example workflow with context shape and icon emphasized

## Infrastructure

 While some things, such as a network, are obviously infrastructure, other things such as a transcode service may or may not be infrastructure depending on the context and the choice of the individual author. Infrastructure is a layered concept. At the top is software[\[5\]](#post-2342-footnote-6) doing something and at the bottom is a collection of silicon chips attached to circuit boards powered by electricity. 

**Infrastructure**: The underlying systems and framework required for the production of the Creative Work; it is generally not specific to a particular Creative Work.

### Infrastructure Shape

 The primary shape for infrastructure is a capsule shape.

![Shape, rectangle, square

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-rectangle-square-description-automaticall-1.png) 

 Figure ‑ Infrastructure shape

 Infrastructure shapes can be optionally associated with the tasks, etc., that use the infrastructure using either one of the boundaries shown in Figure 5‑21 or the association connector shown in Figure 5‑19.

### Infrastructure Icons

 The Visual Language icons allow for the identification the intrinsic nature of a piece of infrastructure, as opposed to its use. The current set of infrastructure icons are:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-139.png) 

 Figure ‑ Infrastructure icons

 Examples of the use of these icons are:

| **Icon**                | **Examples**                         |
| ----------------------- | ------------------------------------ |
| Artificial Intelligence | QC, speech to text                   |
| Camera                  | Sony, Blackmagic, Red                |
| Capture Storage         | CF Card, mag                         |
| Cellular Network        | 5G, 4G                               |
| Cloud                   | AWS, GCP, Azure, private             |
| Compute Resources       | Server, GPU, CPU                     |
| Database                | App, FileMaker, Oracle               |
| Electronic Mail         | Outlook, Gmail                       |
| Ethernet                | 10 GigE                              |
| Fiber Optic Network     | FTTP                                 |
| Machine Learning        | Pattern recognition                  |
| Messaging System        | AMQP                                 |
| Microservice            | Encode, decode                       |
| Network infrastructure  | Facility, company                    |
| Orchestration           | Render, video encoding, archiving    |
| Production Consumables  | Gaffer’s tape, construction material |
| Production Equipment    | Lights, cameras, microphones         |
| Software Application    | Script writing, CG, editing          |
| Storage                 | Hard disk, cloud, USB                |
| Wi-Fi Network           | 802.11b                              |
| Workflow Manager        | Zapier, tray.io                      |
| Workstation             | Lenovo, HP                           |
| Transient Storage       | USB drive portable RAID              |
| Working Storage         | NAS, SAN                             |
| Long-term Storage       | Tape, cloud                          |

### Infrastructure Labels

 When a specific icon is not available or more information is required, infrastructure labels are used to further identify the type of infrastructure. The current set of infrastructure labels are listed in Appendix A. While not comprehensive, the set will grow over time.

### Example Use of Infrastructure Shape, Label, and Icon

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-140.png) 

 Figure ‑ Example workflow with infrastructure shapes emphasized

### Physical Infrastructure

 The 2030 Vision focuses on the migration from traditional physical infrastructure to a new infrastructure of cloud-based services and resources. However, many parts of production workflows are intrinsically physical activities which rely on physical equipment and infrastructure. We also regard these facilities and equipment as infrastructure.

### Message Bus

 A message bus is a piece of infrastructure that manages message passing. A message bus is represented by a double ended arrow shape (as opposed to a double ended line). 

![Table

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/table-description-automatically-generated-1.png) 

 Figure ‑ Message bus shape

 The recommended practice is that a line representing a message sent over the message bus should have a segment that is inside the message bus shape and runs along its axis. A line representing a message not sent over the message should either not be inside the message bus shape or should cross at right angles.

### Security

 The security architecture consists of services which are represented by the infrastructure shape except for the following services.[\[6\]](#post-2342-footnote-7) 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-141.png) 

 Figure ‑ Security Icons

## Thing Shape

 In some instances, it is useful to add something to a diagram where other shapes in the visual language are not suitable. One example is where an element of a diagram is not well enough defined and would be replaced later with something more specific. The Thing shape, a non-specific shape, can be used in those circumstances.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-142.png) 

 Figure ‑ Thing shape

 The Thing shape has no semantic meaning. 

 It is used in the next section where the focus of the explanation is the line constructs of the language. 

## N Shapes

 There are points in a workflow where you can’t determine the number of tasks, assets, context, participants, and infrastructure until you are a given point. For example, the number of encoding tasks in a dailies workflow can’t be determined until the task properties are populated. For this case, we use the n version of the shape. The cardinality is indicated on the lines. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-143.png) 

 Figure ‑ N shape

# The Meaning of Lines

 This section defines how lines are formatted and used to convey meaning. To the extent that lines connect two things, they depict relationships that are defined in the ontology. Each line type may correspond to more than one of those relationships. So, the mapping from the ontology to the Visual Language is many to one and, therefore, not in the general case reversible. Certain, constrained categories of diagrams may be reversible. The mapping of relationships to line types is detailed in Appendix C.

 The following are used to define the meaning of lines:

* The shape at the end on the line (arrowhead) conveys the primary meaning
* The line being solid, dashed or dotted conveys secondary meaning

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-144.png) 

 Figure ‑ Types of arrowheads and lines

 The following do not convey meaning within the Visual Language and are reserved for use by users:

* Line weight  
   * E.g., weight can be used to emphasis parts of the diagram
* Line color or shade  
   * E.g., color can be used as an aid to explanation by identifying certain lines

### Variations of Arrowheads and Lines

 The filled versions of the unfilled arrowheads are assigned the same meaning as the original. Although it is not a recommended format, limitations of the drawing application may make a filled version unavoidable.

 Other arrowheads and line types are reserved either for future use or to avoid ambiguity.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-145.png) 

 Figure ‑ Reserved arrowheads and lines

## Flow

 A _Flow_ is defined to be movement, for example progress through a workflow. 

 A _Bidirectional flow_ is a flow occurring in both directions between two entities where the nature of the flow in each direction is identical.

 Flow might be, for example, the sequence of tasks in a workflow or the progression of one asset to assets derived from it. The specific meaning of flow in a diagram depends on the type of diagram and the author’s intent. What the Visual Language shows without further annotation or explanation is a general flow.

 The flow arrowhead is a filled arrow.

![Shape

Description automatically generated with low confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-description-automatically-generated-with-lo-2.png) 

 Figure ‑ Flow arrowhead

 In its simplest form, flow is a way of connecting components with directionality (both unidirectional and bidirectional). 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-146.png) 

 Figure ‑ Types of flow representations

 In Figure 5‑4(a), the flow is from A to B.

 In Figure 5‑4(b), the flow is both from A to B and from B to A. The double ended arrow means the flow is the same in both directions. For example, VFX files are exchanged between different VFX departments. 

 In Figure 5‑4(c), the flow is from A to B is of a different type to the flow from B to A. For example, OCF are sent from dailies to a transcoding service and proxy files are sent back to dailies.

 Whether the construct of Figure 5‑4(b) or the construct of Figure 5‑4(c) is the most appropriate is the decision the author makes.

 When flow is from one element to more than one other element, the arrangement of the lines has significance.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-147.png) 

 Figure ‑ (a) One to one (unicast) and (b) one to many (multicast) flows[\[7\]](#post-2342-footnote-8) 

 Figure 5‑5 illustrates different ways of showing flow from one thing to more than one other thing. In Figure 5‑5(a), the flow from Thing X to Thing A, Thing B and Thing C are independent of each other, and they could be of a different type. In Figure 5‑5(b), the flow from Thing X to Thing A, Thing B and Thing C is the same.

 In Figure 5‑5, the flows can be bidirectional (see Figure 5‑4) however if the flows in Figure 5‑5(b) are bidirectional, the result is clearer if it is drawn as:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-148.png) 

 Figure ‑ Multi-way flow

 To represent flow which is guidance or influence as to how a task is to be conducted. The guidance/influence line is a dashed line with a solid arrow. For example, the creative vision of the director is made manifest in editorial. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-149.png) 

 Figure ‑ Guidance or influence

### Conditional nodes

 A _conditional node_ is a point in a flow where branching can occur based on the state of the system at the time that the node is reached.

 A _forcing factor_ is an external event that forces one path out of the conditional node to be taken regardless of the state of the system.

 Flows may have points where the flow cannot proceed until an event has happened. For this, we use a conditional node where a condition is evaluated, and the flow progresses accordingly. It is not a task itself; it is the assessment of the state after a task or series of tasks. Figure 5‑8 shows some examples. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-150.png) 

 Figure ‑ Examples of decision points

 In Figure 5‑8(a), the flow is managing data from a camera. The camera data that has been unloaded from the data card is sent to the cloud, but the data card can only be reformatted when the transfer has completed. Since the “no” path connects directly back to the conditional node, this is a wait loop.

 In Figure 5‑8(b), the flow has a decision point where, if the director approves color the conform can commence, and if the director does not approve color the color correction has to be repeated.

 Figure 5‑8(c) is like Figure 5‑8(b) but the decision is also influenced by an event. Here the production has got to the last shot of the day but cannot wrap for the day until the director has a take that they like. However, in this scenario the scene is an exterior shot, and at sunset, the light is lost forcing a wrap for the day even if the director does not get the take. 

### Convergence

 When flows converge it may be necessary to show whether the convergence is blocking or non-blocking. 

_Blocking Convergence_ is a point where several flows converge, and flow cannot proceed until all the flows that converge have reached the convergence point.

_Non-blocking Convergence_ is a point where several flows converge, and flow can proceed when any of the flows reach the convergence point.

 To represent convergence, we borrow the “summing junction” and “or” shapes from traditional flowcharts.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-151.png) 

 Figure ‑ Blocking convergence

 In the blocking flow, the next activity cannot start until activities X, Y, and Z have completed.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-152.png) 

 Figure ‑ Non-blocking convergence 

 In the non-blocking flow, the next activity can start as soon as one of activities X, Y, and Z completes.

 What it means for a flow to reach the convergence point is up to the diagram author.

## Messages

 A _Message_ is a piece of data exchanged between entities such as workflow management elements regarding the control of a workflow.

 For each message, one entity is the sender, and the other entity is the receiver. The Visual Language defines two types of message line. A message is sent from a sender to a receiver and a response (if any) is sent from the receiver to the sender. 

 The message line is a solid line with an open half arrowhead.

![Shape

Description automatically generated with low confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-description-automatically-generated-with-lo-3.png) 

 Figure ‑ Message arrowhead

 The position of the half arrowhead has meaning.

* The message line has the half arrowhead above a horizontal message line or to the right of a vertical message line
* The response line has the half arrowhead below a horizontal message line or to the left of a vertical message line
* A message line can be double ended and the convention of orientation of the arrows should be followed

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-153.png) 

 Figure ‑ Message representations

 Figure 5‑12(a) shows the representation of a message and an associated response. This format allows space to add descriptions to the lines. 

 Figure 5‑12(b) shows an abbreviated form where one double ended line is used. 

 Figure 5‑12(c) shows a message with no response. 

 Figure 5‑12(d) shows the orientation of the arrow heads when the message lines connect with a shape on the top or bottom. 

 Since the orientation of the arrowhead is significant, a pair of lines are needed if either Thing could be a sender. 

## Data movement 

_Data movement_ is the movement of data from one location to another. The movement may be literal, data is copied from one storage location to another, or notional such as the movement of data to a task where the literal movement may be no more than loading the data into system memory.

 The data movement line is a solid line with a wide unfilled arrowhead, it indicates the movement of data from one place to another. The arrowhead must be wider than the flow arrow to avoid confusion if the diagramming application does not provide open arrowheads.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-154.png) 

 Figure ‑ Data movement arrowhead

 As with flow, a doubled ended data movement line means the same type of data moves in both directions. If a different type of data moves one way than the other, two lines should be used.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-155.png) 

 Figure ‑ Data movement

_Information movement_ is the transfer of information that is not data or metadata. For example, the information “the art director says that red lighting won’t work with the costumes in this scene” is sent to the cinematographer or the information “the producer thinks it needs a bake-off around page 30” is sent to the writer. For this purpose, the information movement format is available.

 The information input line is a data movement line that is dotted.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-156.png) 

 Figure ‑ Information movement

## API Calls

 The use of an API call can be indicated in a diagram using the API call line which is a double line with a solid arrow head on one end, the server end. 

![Graphical user interface, application

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/graphical-user-interface-application-description-2.png) 

 Figure ‑ API Call

## Data Communications Links

 A _Data Communications Link_ is a means of connecting one location to another for the purpose of transmitting and receiving digital information. 

 Diagrams that show infrastructure may need to show data communications links. The data communications link line is a solid line with unfilled diamonds at both ends. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-157.png) 

 Figure ‑ Data communications link

 Figure 5‑17(b) shows how the data communications link, a piece of infrastructure, and data movement, the use of the data communications link, should be shown separately. 

## Associations

 An _Association_ is a way of connecting two or more things in a diagram to show they have a relationship between each other. The word “relationship” is used here in the general sense of that word and not in the formal ontological meaning. Ontological relationships can be expressed using the association construct, however mapping from the ontology to an association is many to one and, therefore, not in the general case reversible.

 Associations can be shown using the association line or the grouping shapes. 

### Association Connector

 The association line is a solid line with unfilled circles on both ends.

![Graphical user interface, application

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/graphical-user-interface-application-description-3.png) 

 Figure ‑ Association connector

 This construct is used, for example, in Figure 5‑19 to indicate that the five participants take part in the task. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-158.png) 

 Figure ‑ Association connector example

 Figure 5‑19 uses the expediency of nesting the participant shapes to indicate they are a group and then using a single association connector.

 Another example of the use of the association connector is when infrastructure is represented in a diagram and is associated only with specific elements as is shown in Figure 5-19 where tasks 1, 2 and 3 use cloud A and task 4 uses cloud B.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-159.png) 

 Figure ‑ Association of tasks with infrastructure components

 If all the tasks used both cloud A and cloud B, the association connector might not be needed.

### Grouping

 A group is a boundary drawn around elements in a diagram. It is a shape made up of horizontal and vertical lines with corners that are not radiused. In the simplest case, that is a rectangle, but it can include “T” shapes, “L” shapes and many others. Please note this description of the group construct is not identical to the ontology definition. 

 Different types of boundary lines are used to represent formal and informal groupings:

* The formal boundary is a solid line. This construct is used when there is an association between the elements within the boundary. For example, the elements are part of a department, or are part of a workflow.
* The informal or informational boundary is a dashed line. This construct is used when elements are grouped to add clarity or additional information to a diagram.

 A formal boundary has a semantic meaning within the context of the diagram. For example, it groups together the tasks and participants in a department. 

 An informal bound is used to group items where the grouping is more general in nature. For example, it groups together elements that are part of post-production. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-160.png) 

 Figure ‑ Boundaries

 In Figure 5‑21, it is important to know which tasks are being performed by which department and who the participants are, and it is useful to know which elements are in principal photography and which are in post-production.

_Recommended practice: To distinguish a group from other_ lines in the diagram, the recommended practice is to use thicker lines of a lighter tone for groups and place the group shape behind all other shapes in the diagram.

 As noted above, there is no requirement for a boundary to be rectangular, but the corners must be right angles (and not radiused), and the lines horizontal or vertical.[\[8\]](#post-2342-footnote-9) 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-161.png) 

 Figure ‑ Example of a non-rectangular boundary 

## Example uses of lines

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-162.png) 

 Figure ‑ Example workflow with lines emphasized

# Drawing constructs and annotations

## Annotations

 It is often necessary to add explanation within a diagram other than the text that goes within a shape. For this we use callouts. 

* The callout line has an open arrowhead on one end
* The callout text is in italics

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-163.png) 

 Figure ‑ Callout 

 The recommended practice is that the callout line is lighter in shade or thickness than other lines

## Keys and Titles

 Diagrams also need keys and titles as shown in Figure 6‑2.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-164.png) 

 Figure ‑ Diagram key and title

## Expanded Views

 In many cases the subject of a diagram has details that are not shown. For example, many tasks process OCF including dailies. It may not be necessary for the purpose of a particular diagram to show all the tasks that make up dailies, and instead it is represented as a single task, However, it may be required to show those sub-tasks or the presence of those subtasks.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-165.png) 

 Figure ‑ Expanded and contracted views

 The representation mimics a “click through” user interface.

 A “+” symbol in the top right corner of an element means it can be expanded. In Figure 6‑3(a) the “+” in the top right of the Thing box indicates that Thing is made of sub-Things. 

 A “-” symbol in the top right corner of an element means the expansion is shown somewhere else either in the same diagram or elsewhere. There is no requirement as to where to place the expansion element in the diagram.

 In Figure 6‑3(b) the expansion is shown in the group of sub-Things which is on the same page (in the virtual or literal sense) and a line of the same shade, color and thickness as the group shape connects the two.

 In Figure 6‑3(c) the expanded view is in another place and a reference is shown to the location of the expansion. 

 In an interactive diagram, the “+” symbol would be a clickable link. 

1. Labels

 The following sections outline some recommended labels to use while creating workflow diagrams. The terms and definitions come from the MovieLabs Ontology for Media Creation.

* 1. Asset Labels

 The following a list of asset labels and icons if appropriate:

| **Asset Labels**            | **Icon**                                                                                              | **Definition**                                                                                                                                                       |
| --------------------------- | ----------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Image                       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-166.png) | A representation of a 2-dimensional picture.                                                                                                                         |
| Digital Image               | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-167.png) | A 2-dimensional picture stored digitally with values representing color, depth (distance from the point of capture), and alpha (transparency) at given pixels (x, y) |
| Analog Image                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-168.png) | A 2-dimensional pictured stored in an analog form such a drawing on paper, an image on 35mm film.                                                                    |
| Moving Image                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-169.png) | A temporally ordered sequence of images.                                                                                                                             |
| Analog Moving Image         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-170.png) | A temporally ordered sequence of Analog Images                                                                                                                       |
| Digital Moving Image        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-171.png) | A temporally ordered sequence of Digital Images.                                                                                                                     |
| Audio                       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-172.png) | A representation of sound.                                                                                                                                           |
| Analog Audio                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-173.png) | Sound stored as a continuous waveform.                                                                                                                               |
| Digital Audio               | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-174.png) | Sound stored as a set of digital values                                                                                                                              |
| Audio Visual                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-175.png) | A Moving Image with Audio synchronized to the images.                                                                                                                |
| Analog Audio Visual         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-176.png) | An Analog Moving Image with synchronized Analog Audio.                                                                                                               |
| Digital Audio Visual        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-177.png) | A temporally ordered sequence of Digital Images with synchronized Digital Audio                                                                                      |
| Document                    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-178.png) | A human readable object containing text and/or images.                                                                                                               |
| Analog Document             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-179.png) | A document stored in an analog form such as on paper.                                                                                                                |
| Digital Document            | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-180.png) | A document stored in a digital form such as a PDF file.                                                                                                              |
| Structured Document         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-181.png) | A Document structured according to a set of rules which are used to parse or understand the document.                                                                |
| Analog Structured Document  | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-182.png) | A structured document stored in an analog form such as on paper.                                                                                                     |
| Digital Structured Document | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-183.png) | A structured document stored in a digital form such as a PDF file.                                                                                                   |

* 1. Task Labels

 The following is a list of task labels. There are no task icons for the first version of the Visual Language.

| **Standard Task Label**              | **Definition**                                                                                                                                   |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Write Script                         | Develop and revise a script.                                                                                                                     |
| Develop Creative Style               | Prepare the look and tone of the production.                                                                                                     |
| Previsualize                         | Creative visuals for the creative elements of the work.                                                                                          |
| Create Set                           | Make a Set for use in a Production Scene.                                                                                                        |
| Capture Technical Reference Material | Capture technical reference material about the state of the shooting environment during production.                                              |
| Perform Scene                        | Perform actions and dialog.                                                                                                                      |
| Shoot                                | Capture a shot.                                                                                                                                  |
| Maintain Continuity                  | Ensure consistency of the narrative in relation to the production across takes and time.                                                         |
| Create Editorial Dailies             | Create reviewable video and or audio of a given day's work for the editorial process.                                                            |
| Edit                                 | Assemble shots into a sequence conforming to the narrative.                                                                                      |
| Create Visual Effects                | Integrate and manipulate live action and/or CG footage to create imagery for the finishing process.                                              |
| Create Titles                        | Create imagery for the contributions to the creative work.                                                                                       |
| Conform Finish                       | Assemble the final imagery consisting of captured high-resolution material, VFX shots, titling, and opticals based on final editorial decisions. |
| Master                               | Create the various packages for archive and distribution.                                                                                        |
| Distribute                           | Make the creative work available to a public audience.                                                                                           |

* 1. Participant Labels

 The following is a list of Participant Labels:

| **Standard Participant Label** | **Icon**                                                                                                                                                                                                     | **Definition**                                                                                                                                               |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Director                       | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-23.png) | People are the individuals that are associated with the production.                                                                                          |
| First Assistant Director       | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-24.png) | Person who leads the production of motion pictures and sets whatever is heard or seen in the final film.                                                     |
| Producer                       | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-25.png) | Person that organizes the pre-production preparation and the flow of production activity on-set.                                                             |
| Showrunner                     | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-26.png) | Person who makes key decisions for the Creative Work on behalf of the studio or broadcaster.                                                                 |
| Actor                          | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-27.png) | Person who portrays a Character.                                                                                                                             |
| Voice Actor                    | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-28.png) | Person who records primary dialogue for a character in the script, often in animated works                                                                   |
| Screenwriter                   | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-29.png) | Person that develops the story either through adapting original written works or creating a new screenplay.                                                  |
| Editor                         | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-30.png) | Person that works with the director and Producer to edit the final cut of the creative work.                                                                 |
| Director of Photography        | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-31.png) | Person responsible for all the elements that affect what the camera is able to capture (i.e., lighting, composition, exposure, etc.).                        |
| Composer                       | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-32.png) | Person that creates the musical score that accompanies the production.                                                                                       |
| Sound Mixer                    | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-33.png) | Person that records, dubs, synchronizes, and scores sound in a production.                                                                                   |
| VFX Supervisor                 | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-34.png) | Person responsible for achieving the creative aims of the director/producers of a project through the use of Visual Effects.                                 |
| Production Designer            | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-35.png) | Person that creates and develops the overall look, atmosphere and emotion that move the story.                                                               |
| Set Designer                   | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-36.png) | Person that architects the structures or spaces required by the production designer.                                                                         |
| Casting Director               | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-37.png) | Person that collaborates with producers, directors, network, and studios executives to cast the talent per role.                                             |
| Stunt Coordinator              | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-38.png) | Person that creates and engineers stunts and hires the stunt performers.                                                                                     |
| _Camera Department_            | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-39.png) | Organization responsible for setting up and operating the cameras during a production.                                                                       |
| _Camera Unit_                  | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-40.png) | Organization responsible for shooting some element of a Scene, e.g., a Main Unit or Second Unit.                                                             |
| _Costume Department_           | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-41.png) | Organization responsible for all of the clothing and costumes worn by the cast in a production.                                                              |
| _Editorial Department_         | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-42.png) | Organization responsible for the artistic assembly of the Creative Work working with the director and producers.                                             |
| _Visual Effects_               | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-43.png) | Organization responsible for the creation and manipulation of image data to add or remove objects, environments, characters, and effects to a creative work. |
| _Production Office_            | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-44.png) | Organization responsible for all of the administrative and management tasks in a production.                                                                 |
| _Archive_                      | ![Diagram Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-with-45.png) | Organization that provides preservation of and access to digital and physical assets.                                                                        |
| _Encoding_                     | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-184.png)                                                                                                        | Service to compress, index, encrypt and package media assets.                                                                                                |
| _Transfer_                     | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-185.png)                                                                                                        | Service to move or copy media assets between locations.                                                                                                      |
| _Rendering_                    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-186.png)                                                                                                        | Service to process content creation setups (2D and 3D) to deliver image assets.                                                                              |

* 1. Context Labels

 The following is a list of Context Labels:

| **Name**                       | **Icon**                                                                                                                                                                                                                    | **Definition**                                                                                                                                                                                          |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Location                       | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-15.png) | A particular place or position either in either the real world or the narrative world.                                                                                                                  |
| Narrative Location             | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-16.png) | A location specified or implied by the narrative.                                                                                                                                                       |
| Production Location            | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-17.png) | A real place that is used to depict the Narrative Location or used for creating the production.                                                                                                         |
| Prop                           | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-187.png)                                                                                                                       | A named object related to or interacting with characters that is implied or understood to be necessary for the narrative.                                                                               |
| Narrative Prop                 | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-188.png)                                                                                                                       | A Prop as specified or implied by the narrative.                                                                                                                                                        |
| Production Prop                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-189.png)                                                                                                                       | A Depiction of the Narrative Prop.                                                                                                                                                                      |
| Set Dressing                   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-190.png)                                                                                                                       | Objects used on set to create and enhance the environment.                                                                                                                                              |
| Narrative Wardrobe             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-191.png)                                                                                                                       | The clothing for a Character in the narrative.                                                                                                                                                          |
| Costume                        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-192.png)                                                                                                                       | The clothing used in a Portrayal of a Character in the production.                                                                                                                                      |
| Storyboard                     | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-193.png)                                                                                                                       | A series of images that forms a visual representation of some part of the narrative.                                                                                                                    |
| Animated Storyboard            | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-194.png)                                                                                                                       | A moving image produced from the individual images of a Storyboard.                                                                                                                                     |
| Creative Reference Material    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-195.png)                                                                                                                       | Images or other material used to inform the creation of a production element, to help convey a tone or look, etc.                                                                                       |
| Technical Reference Material   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-196.png)                                                                                                                       | Images and other material used to inform the execution of the production.                                                                                                                               |
| Shooting Set                   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-197.png)                                                                                                                       | A fixed, specified Location for shooting/filming.                                                                                                                                                       |
| Production Set                 | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-198.png)                                                                                                                       | An environment built for use on a Shooting Set.                                                                                                                                                         |
| Scene                          | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-199.png)                                                                                                                       | A section of the Script typically defined by a unity of location or time but could be based on a different single narrative context where a montage or multiple locations make up the scene.            |
| Narrative Scene                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-200.png)                                                                                                                       | Taken from the narrative itself and traditionally defined by creative intent and typically a unity of time, place, action, or theme.                                                                    |
| Production Scene               | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-201.png)                                                                                                                       | Defined either by explicit divisions in the structure of the Script, e.g., by a Slugline, or by additional capture for use in the Creative Work that is not tied to any particular Scene in the Script. |
| Slugline                       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-202.png)                                                                                                                       | A line within a screenplay written in all uppercase letters to draw attention to specific script information.                                                                                           |
| Scene Number                   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-203.png)                                                                                                                       | A number tied to the Slugline when a Script is locked.                                                                                                                                                  |
| Scene Header                   | Future Version![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-204.png)                                                                                                         | Used when referring to the Production Scene. It is generally synonymous with Slugline and is used to divide a Script into Production Scenes.                                                            |
| Character                      | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-18.png) | A sentient entity (usually a person but not always) in the script whose specific identity is consequential to the narrative. A Character is generally identified by a specific name.                    |
| Concept                        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-205.png)                                                                                                                       | An exploratory representation of something from the narrative.                                                                                                                                          |
| Concept Art                    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-206.png)                                                                                                                       | Images that illustrate ideas for potential depictions of elements of the creative intent.                                                                                                               |
| Depiction                      | Future Version                                                                                                                                                                                                              | The representation of something from a narrative entity by a production entity in the Creative Work, specified or implied by the Script.                                                                |
| Portrayal                      | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-19.png) | The Depiction of a Character.                                                                                                                                                                           |
| Creative Work                  | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-20.png) | A uniquely identified production.                                                                                                                                                                       |
| Identifier                     | Future Version                                                                                                                                                                                                              | An identifier uniquely identifies an entity within a particular scope.                                                                                                                                  |
| Slate                          | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-21.png) | Used to capture key identifying information about what is being recorded on any given setup and take.                                                                                                   |
| Scene Descriptor               | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-22.png) | An alphanumeric reference to the Production Scene being recorded.                                                                                                                                       |
| Setup                          | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-23.png) | The unique camera configuration which encompasses a cameras geo-location, positioning, lens, or other camera settings.                                                                                  |
| Take                           | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-24.png) | A discrete capture event with a specified beginning and end.                                                                                                                                            |
| Slate UID                      | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-25.png) | An alphanumeric code that uniquely identifies a single clip by combining the Scene Descriptor, Setup, and Take.                                                                                         |
| Camera Identifier              | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-26.png) | An identifier for the camera responsible for the capture, usually related to the role and responsibility of the group operating it and usually a single upper-case letter starting with A.              |
| Camera Unit                    | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-27.png) | A group of Participants responsible for shooting some element of a Scene, e.g., Main Unit or Second Unit.                                                                                               |
| Camera Roll                    | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-28.png) | Identifier for a group of events captured together on the same camera.                                                                                                                                  |
| Sound Roll                     | ![A picture containing text, receipt, screenshot Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-receipt-screenshot-de-29.png) | Identifier for a group of audio events captured together on the same recording device.                                                                                                                  |
| Shoot Date                     | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-207.png)                                                                                                                       | The date of capture.                                                                                                                                                                                    |
| Shoot Day                      | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-208.png)                                                                                                                       | The number of the day on the shooting schedule.                                                                                                                                                         |
| Shot                           | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-209.png)                                                                                                                       | A discrete unit of visual narrative with a specified beginning and end.                                                                                                                                 |
| Sequence                       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-210.png)                                                                                                                       | An ordered collection of media used to organize units of work.                                                                                                                                          |
| Editorial Sequence             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-211.png)                                                                                                                       | A sequence of shots linked to creative intent.                                                                                                                                                          |
| VFX Shot                       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-212.png)                                                                                                                       | A Shot that has been identified as requiring VFX work.                                                                                                                                                  |
| VFX Sequence                   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-213.png)                                                                                                                       | A unit of work made up of an ordered series of VFX shots.                                                                                                                                               |
| Animation Shot                 | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-214.png)                                                                                                                       | A Shot that has been identified as requiring Animation work.                                                                                                                                            |
| Animation Sequence             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-215.png)                                                                                                                       | A unit of work made up of an ordered series of Animation shots.                                                                                                                                         |
| Color Sequence                 | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-216.png)                                                                                                                       | A sequence of shots with color grading characteristics linked to creative intent.                                                                                                                       |
| Sequence Chronology Descriptor | Future Version                                                                                                                                                                                                              | Describes how a series of Shots is used to generate a Sequence.                                                                                                                                         |

* 1. Infrastructure Labels

 The following a list of infrastructure labels and icons if appropriate:

| **Asset Labels**        | **Icon**                                                                                                                                                                                                    | **Definition**                                                                                                                                                                                                                      |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Workflow Manager        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-217.png)                                                                                                       | A system that manages and assigns tasks in a production.                                                                                                                                                                            |
| Orchestration Manager   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-218.png)                                                                                                       | A system that receives messages from the workflow manager to orchestrate resources to complete tasks in a Software Defined Workflow.                                                                                                |
| Cloud                   | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-219.png)                                                                                                       | Processing, storage, networks, and other fundamental computing resources provisioned to be made available on demand where the user is able to deploy and run arbitrary software without managing the underlying physical resources. |
| Public Cloud            | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-220.png)                                                                                                       | Cloud resources provisioned for and available to many unaffiliated organizations and individuals. It is typically owned, managed, and operated by a third party.                                                                    |
| Private Cloud           | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-221.png)                                                                                                       | Cloud resources provisioned for exclusive use by a single organization. It may be owned, managed, and operated by the organization, a third party, or some combination of them                                                      |
| Workstation             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-222.png)                                                                                                       | An individual computer, typically high powered and used for the processes like editing or designing 3D models.                                                                                                                      |
| Remote Desktop          | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-223.png)                                                                                                       | The use of one machine (a laptop, desktop, or thin client) to connect over a network to another, which it controls as if it were local.                                                                                             |
| Network Infrastructure  | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-224.png)                                                                                                       | The underlying network hardware and software required to connect devices, production sites and services                                                                                                                             |
| Private Network         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-225.png)                                                                                                       | A network provisioned for exclusive use by a single organization. It may be owned, managed, and operated by the organization, a third party, or some combination of them.                                                           |
| Public Network          | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-226.png)                                                                                                       | A network provisioned for use by the general public. for and available to many unaffiliated organizations and individuals. It is typically owned, managed, and operated by a third party.                                           |
| Cellular Network        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-227.png)                                                                                                       | A high speed radio data network using 4th, 5th or later generation cellular standards.                                                                                                                                              |
| WiFi                    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-228.png)                                                                                                       | A family of wireless local area networking protocols.                                                                                                                                                                               |
| Ethernet                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-229.png)                                                                                                       | A family of wired network technologies used in local area networks (LAN), metropolitan area networks (MAN) and wide area networks (WAN).                                                                                            |
| Fiber Optic             | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-230.png)                                                                                                       | A family of network technologies using optical fiber to provide high speed data communications over long distances with immunity to electromagnetic interference.                                                                   |
| Edge Compute            | Future version                                                                                                                                                                                              | A system where compute resources are placed at the edge of the cloud or network, and logically close to the user.                                                                                                                   |
| Edge Storage            | Future version                                                                                                                                                                                              | A system where storage resources are placed at the edge of the cloud or network, and logically close to the user. Edge storage can be used to cache data to avoid network latency in data retrieval                                 |
| Messaging System        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-231.png)                                                                                                       | A Message Bus and its associated Message Brokers.                                                                                                                                                                                   |
| Software Service        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-232.png)                                                                                                       | An Application that runs within the cloud.                                                                                                                                                                                          |
| Microservice            | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-233.png)                                                                                                       | A small discrete application that performs one very specific task or operation when called. These are often coupled together to create workflows.                                                                                   |
| Electronic Mail         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-234.png)                                                                                                       | Responsible for sending and receiving electronic mail.                                                                                                                                                                              |
| Database                | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-235.png) ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-236.png) | A system for storing, searching, and retrieving structured data.                                                                                                                                                                    |
| Storage                 | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-237.png) ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-238.png) | A system to store and retrieve data.                                                                                                                                                                                                |
| Software Application    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-239.png)                                                                                                       | A monolithic application typically designed for a particular area of production, such script markup, picture editorial or CG modelling.                                                                                             |
| Machine Learning        | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-240.png)                                                                                                       | Processes and algorithms that enable a computational system to automatically perform a task based on training data.                                                                                                                 |
| Production Equipment    | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-241.png)                                                                                                       | Electronic or mechanical equipment used during the on-set or location shooting task.                                                                                                                                                |
| Production Consumables  | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-242.png)                                                                                                       | A commodity or disposable item that is used during the on-set or location shooting task.                                                                                                                                            |
| Capture Storage         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-243.png)                                                                                                       | A system for storing, and retrieving data from a capture device.                                                                                                                                                                    |
| Transient Storage       | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-244.png)                                                                                                       | A system for storing and transferring data between locations.                                                                                                                                                                       |
| Working Storage         | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-245.png)                                                                                                       | A system for storing, and retrieving data during the production process.                                                                                                                                                            |
| Final Storage           | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-246.png)                                                                                                       | A system for storing, and retrieving data after a production is complete.                                                                                                                                                           |
| Artificial Intelligence | ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-247.png)                                                                                                       | The ability of a computational system to autonomously perform tasks commonly associated with intelligent beings.                                                                                                                    |

1. Best Practices

 The following is a set of best practices when building diagrams, apps, and dashboards using the Visual Language. 

* 1. Layout Practices

 The recommended practice for laying out diagrams for workflows are:

* Primary flow is left to right (horizontal) or top to bottom (vertical)
* Diagrams are primarily either horizontal or vertical

 Flow can be emphasized by a cascading arrangement flowing left to right. 

 To avoid diagrams that are too wide or too tall it may be necessary to “fold” a flow. The recommended practice is that the direction of flow should be maintained. e.g., left to right before and after the fold rather than left to right up to the fold and then right to left beyond the “fold.”

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-248.png) 

 Figure B‑1 (a) Recommended way to fold a horizontal flow, (b) not recommended

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-249.png) 

 Figure B‑2 (a) Recommended way to fold a vertical flow, (b) not recommended

* 1. Using Fixed Canvas Sizes

 We suggest you use the following canvas sizes as a starting point. This will allow you to declare the intended viewing paradigm for your diagram or workflow:

* 1. mobile: 360x640 (9:16) portrait  
   2. mobile: 640x360 (16:9) landscape / Streaming  
   3. desktop 1: 1920x1080 (16:9) / Streaming  
   4. desktop 2: 1366x768 (16:9)  
   5. tablet: 768x1024 (3:4) portrait  
   6. tablet: 1024x768 (4:3) landscape  
   7. Streaming: 2560×1440 (16:9)  
   8. Streaming 4K: 3840×2160 (16:9)

 Using a fixed Canvas size in tools like Lucid Chart and disabling auto-scale will allow you to see how users will experience your diagrams on their various devices. 

* 1. Shape Sizes

 All shapes and icons are resizable given they are based on vector graphics. Once you determine which canvas you are going to use then you can the guide to determine what size you want for the shape based on how many objects you intend to show in your workflow. First you can start with the concept there are three shape sizes: Small, Medium, and Large. You can also think of shape size in terms of scale as seen below if you are doing application development.

![Graphical user interface

Description automatically generated with medium confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/graphical-user-interface-description-automaticall-2.png) ![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-250.png) 

 Figure B‑3 Shape Scale

 Then you can use the information below to determine how many shapes you can fit on your chosen canvas.

1. Small Task  
   1. mobile: 360x640 (9:16) portrait - 7x17=119  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 13x10=130  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 39x30=1,170  
   4. desktop 2: 1366x768 (16:9) - 28x21=588  
   5. tablet: 768x1024 (3:4) portrait - 15x28=420  
   6. tablet: 1024x768 (4:3) landscape - 21x21=441  
   7. Streaming: 2560×1440 (16:9) - 52x40=2,080  
   8. Streaming 4K: 3840×2160 (16:9) - 79x65=5,135  
   9. New Laptops CES: 1920x1280 (3:2) - 39x35=1,365  
   10. New Laptops CES: 2560x1600 (16:10) - 52x44=2,288
2. Medium Task  
   1. mobile: 360x640 (9:16) portrait - 3x8=24  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 6x5=30  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 19x15=285  
   4. desktop 2: 1366x768 (16:9) - 14x10=140  
   5. tablet: 768x1024 (3:4) portrait - 7x14=98  
   6. tablet: 1024x768 (4:3) landscape - 10x10=100  
   7. Streaming: 2560×1440 (16:9) - 26x20=520  
   8. Streaming 4K: 3840×2160 (16:9) - 39x30=1,170  
   9. New Laptops CES: 1920x1280 (3:2) - 19x17=323  
   10. New Laptops CES: 2560x1600 (16:10) - 26x22=572
3. Large Task  
   1. mobile: 360x640 (9:16) portrait - 1x4=4  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 3x2=6  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 9x7=63  
   4. desktop 2: 1366x768 (16:9) - 7x5=35  
   5. tablet: 768x1024 (3:4) portrait - 3x7=21  
   6. tablet: 1024x768 (4:3) landscape - 5x5=25  
   7. Streaming: 2560×1440 (16:9) - 13x10=130  
   8. Streaming 4K: 3840×2160 (16:9) - 19x15=285  
   9. New Laptops CES: 1920x1280 (3:2) - 9x8=72  
   10. New Laptops CES: 2560x1600 (16:10) - 13x11=143
4. Small Asset  
   1. mobile: 360x640 (9:16) portrait - 10x17=170  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 17x10=170  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 53x30=1,590  
   4. desktop 2: 1366x768 (16:9) - 37x21=777  
   5. tablet: 768x1024 (3:4) portrait - 21x28=588  
   6. tablet: 1024x768 (4:3) landscape - 28x21=588  
   7. Streaming: 2560×1440 (16:9) - 71x40=2,840  
   8. Streaming 4K: 3840×2160 (16:9) - 106x60=6,360  
   9. New Laptops CES: 1920x1280 (3:2) - 53x35=1,855  
   10. New Laptops CES: 2560x1600 (16:10) - 71x44=3,124
5. Medium Asset  
   1. mobile: 360x640 (9:16) portrait - 5x8=40  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 8x5=40  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 26x15=390  
   4. desktop 2: 1366x768 (16:9) - 18x10=180  
   5. tablet: 768x1024 (3:4) portrait - 10x14=140  
   6. tablet: 1024x768 (4:3) landscape - 14x10=140  
   7. Streaming: 2560×1440 (16:9) - 25x20=500  
   8. Streaming 4K: 3840×2160 (16:9) - 53x30=1,590  
   9. New Laptops CES: 1920x1280 (3:2) - 26x17=442  
   10. New Laptops CES: 2560x1600 (16:10) - 35x22=770
6. Large Asset  
   1. mobile: 360x640 (9:16) portrait - 2x4=8  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 4x2=8  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 13x7=91  
   4. desktop 2: 1366x768 (16:9) - 9x5=45  
   5. tablet: 768x1024 (3:4) portrait - 5x7=35  
   6. tablet: 1024x768 (4:3) landscape - 7x5=35  
   7. Streaming: 2560×1440 (16:9) - 17x10=170  
   8. Streaming 4K: 3840×2160 (16:9) - 26x15=390  
   9. New Laptops CES: 1920x1280 (3:2) - 13x8=104  
   10. New Laptops CES: 2560x1600 (16:10) - 17x11=187
7. Small Context  
   1. mobile: 360x640 (9:16) portrait - 10x17=170  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 17x10=170  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 53x30=1,590  
   4. desktop 2: 1366x768 (16:9) - 37x21=777  
   5. tablet: 768x1024 (3:4) portrait - 21x28=588  
   6. tablet: 1024x768 (4:3) landscape - 28x21=588  
   7. Streaming: 2560×1440 (16:9) - 71x40=2,840  
   8. Streaming 4K: 3840×2160 (16:9) - 106x60=6,360  
   9. New Laptops CES: 1920x1280 (3:2) - 53x35=1,855  
   10. New Laptops CES: 2560x1600 (16:10) - 71x44=3,124
8. Medium Context  
   1. mobile: 360x640 (9:16) portrait - 5x8=40  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 8x5=40  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 26x15=390  
   4. desktop 2: 1366x768 (16:9) - 18x10=180  
   5. tablet: 768x1024 (3:4) portrait - 10x14=140  
   6. tablet: 1024x768 (4:3) landscape - 14x10=140  
   7. Streaming: 2560×1440 (16:9) - 25x20=500  
   8. Streaming 4K: 3840×2160 (16:9) - 53x30=1,590  
   9. New Laptops CES: 1920x1280 (3:2) - 26x17=442  
   10. New Laptops CES: 2560x1600 (16:10) - 35x22=770
9. Large Context  
   1. mobile: 360x640 (9:16) portrait - 2x4=8  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 4x2=8  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 13x7=91  
   4. desktop 2: 1366x768 (16:9) - 9x5=45  
   5. tablet: 768x1024 (3:4) portrait - 5x7=35  
   6. tablet: 1024x768 (4:3) landscape - 7x5=35  
   7. Streaming: 2560×1440 (16:9) - 17x10=170  
   8. Streaming 4K: 3840×2160 (16:9) - 26x15=390  
   9. New Laptops CES: 1920x1280 (3:2) - 13x8=104  
   10. New Laptops CES: 2560x1600 (16:10) - 17x11=187
10. Small Participant  
   1. mobile: 360x640 (9:16) portrait - 9x17=153  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 16x10=160  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 47x30=1,410  
   4. desktop 2: 1366x768 (16:9) - 34x21=714  
   5. tablet: 768x1024 (3:4) portrait - 19x28=532  
   6. tablet: 1024x768 (4:3) landscape - 25x21=525  
   7. Streaming: 2560×1440 (16:9) - 63x44=2,772  
   8. Streaming 4K: 3840×2160 (16:9) - 95x60=5,700  
   9. New Laptops CES: 1920x1280 (3:2) - 47x35=1,645  
   10. New Laptops CES: 2560x1600 (16:10) - 63x44=2,772
11. Medium Participant  
   1. mobile: 360x640 (9:16) portrait - 4x8=32  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 8x5=40  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 23x15=345  
   4. desktop 2: 1366x768 (16:9) - 17x10=170  
   5. tablet: 768x1024 (3:4) portrait - 9x13=117  
   6. tablet: 1024x768 (4:3) landscape - 12x10=120  
   7. Streaming: 2560×1440 (16:9) - 31x20=620  
   8. Streaming 4K: 3840×2160 (16:9) - 47x30=1,410  
   9. New Laptops CES: 1920x1280 (3:2) - 23x17=391  
   10. New Laptops CES: 2560x1600 (16:10) - 31x22=682
12. Large Participant  
   1. mobile: 360x640 (9:16) portrait - 2x4=8  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 4x2=8  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 11x7=77  
   4. desktop 2: 1366x768 (16:9) - 8x5=40  
   5. tablet: 768x1024 (3:4) portrait - 4x7=28  
   6. tablet: 1024x768 (4:3) landscape - 6x5=30  
   7. Streaming: 2560×1440 (16:9) - 15x10=150  
   8. Streaming 4K: 3840×2160 (16:9) - 23x15=345  
   9. New Laptops CES: 1920x1280 (3:2) - 12x8=96  
   10. New Laptops CES: 2560x1600 (16:10) - 15x11=165
13. Small Infrastructure  
   1. mobile: 360x640 (9:16) portrait - 5x17=85  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 10x10=100  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 30x30=900  
   4. desktop 2: 1366x768 (16:9) - 21x21=441  
   5. tablet: 768x1024 (3:4) portrait - 12x28=336  
   6. tablet: 1024x768 (4:3) landscape - 16x21=336  
   7. Streaming: 2560×1440 (16:9) - 40x40=1,600  
   8. Streaming 4K: 3840×2160 (16:9) - 60x60=3,600  
   9. New Laptops CES: 1920x1280 (3:2) - 30x35=1,050  
   10. New Laptops CES: 2560x1600 (16:10) - 40x44=1,760
14. Medium Infrastructure  
   1. mobile: 360x640 (9:16) portrait - 2x8=16  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 5x5=25  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 30x30=900  
   4. desktop 2: 1366x768 (16:9) - 10x10=200  
   5. tablet: 768x1024 (3:4) portrait - 6x14=84  
   6. tablet: 1024x768 (4:3) landscape - 8x10=80  
   7. Streaming: 2560×1440 (16:9) - 20x20=400  
   8. Streaming 4K: 3840×2160 (16:9) - 30x30=900  
   9. New Laptops CES: 1920x1280 (3:2) - 15x17=255  
   10. New Laptops CES: 2560x1600 (16:10) - 20x22=440
15. Large Infrastructure  
   1. mobile: 360x640 (9:16) portrait - 1x4=4  
   2. mobile: 640x360 (16:9) landscape / Streaming: 640×360 - 2x2=4  
   3. desktop 1: 1920x1080 (16:9) / Streaming: 1920×1080 - 7x7=14  
   4. desktop 2: 1366x768 (16:9) - 5x5=25  
   5. tablet: 768x1024 (3:4) portrait - 3x7=21  
   6. tablet: 1024x768 (4:3) landscape - 4x5=20  
   7. Streaming: 2560×1440 (16:9) - 10x10=200  
   8. Streaming 4K: 3840×2160 (16:9) - 15x15=225  
   9. New Laptops CES: 1920x1280 (3:2) - 7x8=56  
   10. New Laptops CES: 2560x1600 (16:10) - 10x11=110  
   11. Icon Sizes

 Like with Shapes, icons are vector graphics and can be re-sized. However, we recommend you stick with three sizes when working:

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-251.png) 

 Figure B‑4 Icon Scale

* * 1. Flow, Group and Properties

 Given all shapes and icons are re-sizable, one way of thinking is to build around three sizes for shapes and icons: Flow, group, and properties. ![Graphical user interface

Description automatically generated with low confidence](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/graphical-user-interface-description-automaticall-3.png) 

 Figure B‑5 Shape Detail Example

**Flow**: This is the smallest size and only has an icon within the shape. For example, if you have a flow of assets and want to distinguish the asset type without using a larger shape you can use the flow size. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-252.png) 

 Figure B‑6 Flow Example

**Group**: This is useful when you have a group of objects that are usually the same shape, and you are showing a medium level of complexity in your workflow diagram. This size allows for an icon and a single line of description. For example, you could have a group of shapes that all have the same icon, and you want one line of text to differentiate the objects. 

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-253.png) 

 Figure B‑7 Group Example

**Properties**: This is useful when you have a small number of objects and you want to show multiple pieces of information for each one. This size allows for an icon and multiple lines of text. For example, you could have a group of participants in a production company, and you want to show their type, name, and title.

![Shape

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/shape-description-automatically-generated-3.png) 

 Figure B‑8 Properties Example

* 1. Showing Context in a Workflow

 Given the complex relationship between context and the various ontology concepts we do not recommend showing them in the Visual Language. To show context we usually create a context window (i.e., on the right-hand side) and include them without any connections. There are usually multiple contexts for any diagram. For example, the context below is a creative work named Hyperspace Madness. The context is also the Scene Beach Run. The context is also the Script named 3 min Short v 3\. The context is also the character named Sven. The context is also the location beach. The context is also the prop communicator. 

![Diagram

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-3.png) 

 Figure B‑9 Context Legend

* 1. Creating Custom Themes or Diagrams

 The final recommended best practice involves using the parts of the Visual Language where we have no set guidelines. 

 This includes the following:

* **Color:** Use line color for lines or shapes to denote a certain grouping like all blue lines are image flows or all red shapes are contractors. Also use color to create themes that match company branding.
* **Line thickness:** Use line thickness to emphasize certain shapes or lines for builds or selection in applications or dashboards.
* **Fontography:** We have specified that all callout text in italics. We have not specified which font type. You can very effectively create separation between concepts using different fonts or using bold or different point sizes. When creating a theme using a consistent font can tie a workflow to your brand or company.
* **Texture/Gradient:** The most common use for texture is for a background to a canvas such as the example below where we used a blueprint background. You can also use texture for the style of a line (i.e., chalk line) or for the fill of an object (gradient).
* **Pattern/Fill:** Whereas texture usually comes from an image file pattern or fill is more of a procedural approach. Filling shapes with colors is one example to create a theme or match a brand. You might use fill to indicate status of a given task (i.e., green complete or red indicating error). For patterns, there are all sorts of patterns like hatch or organic. Patterns can be very effective for differentiation or creating depth.
* **OutlineFX:** OutlineFX can include things like shadow, glow, blur, etc. Not all graphic applications or platforms can generate these FX. These are great for highlighting objects or showing state and are suited for application or dashboard development.

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-254.png) 

 Figure B‑10 Example Basic Theme

![A picture containing text, blackboard, blue

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-text-blackboard-blue-descr-1.png) 

 Figure B‑11 Example Blueprint Theme

![](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/word-image-255.png) 

 Figure B‑12 Example App Theme

1. Visual Language Depiction of Ontology Relationships

 The Part 7 of the Ontology for Media Creation defines a rich set of relationships between categories of workflow elements as well as between specific individual elements. The Visual Language does not provide visually distinct depictions for all of these.

 The tables below describe the visual depictions for some of these relationships. These may be useful to those who are implementing software using the Ontology to model workflows and wish to use the Visual Language in user interfaces. 

 The Ontology defines relationships that can point in either direction. The reciprocal relationship (i.e., back from target to the source) is shown in parentheses.

 Task to Asset Relationships

 These are depicted by the Flow Arrow.

| **Ontology Relationship**         | **Source** | **Target** | **Depiction**              |
| --------------------------------- | ---------- | ---------- | -------------------------- |
| hasInputAsset (isInputAssetFor)   | Task       | Asset      | Flow Arrow (Asset to Task) |
| hasOutputAsset (isOutputAssetFor) | Task       | Asset      | Flow Arrow (Task to Asset) |

 Participant to Task Relationships

 In the Ontology, an element called a Role connects Tasks and Participants. In the Visual Language, when a Role connects a Participant and a Task, an Association Line can be used to depict it.

| **Ontology Relationship**              | **Source** | **Target**  | **Depiction**    |
| -------------------------------------- | ---------- | ----------- | ---------------- |
| hasRoleParticipant (isParticipantRole) | Role       | Participant | Association Line |
| hasRoleTask (isTaskInRole)             | Role       | Task        |                  |

 Context Relationships

 The Ontology defines as generic Media Creation Context, as well as more specific Production Context and Narrative Context elements. These group together the set of specific components that define the Context. In the Visual Language, the Context can be depicted as a window containing a set of Context components as described in Section B.5.

| **Ontology Relationship**         | **Source**    | **Target**              | **Depiction**                                   |
| --------------------------------- | ------------- | ----------------------- | ----------------------------------------------- |
| has<\*>Context (is<\*>ContextFor) | (any element) | <\*>Context             | Presence of a context window                    |
| hasContextComponent               | <\*>Context   | (any Context component) | Presence of the Context component in the window |

 Grouping and Granularity Relationships

 The Ontology can express the granularity in which Tasks, Assets and Participants can be further decomposed into components or grouped together. In the Visual Language the decomposition can be depicted using an Expanded View.

| **Ontology Relationship**                          | **Source**  | **Target**  | **Depiction** |
| -------------------------------------------------- | ----------- | ----------- | ------------- |
| hasTaskComponent (isTaskComponentOf)               | Task        | Task        | Expanded View |
| hasAssetComponent (isAssetComponentOf)             | Asset       | Asset       | Expanded View |
| hasParticipantComponent (isParticipantComponentOf) | Participant | Participant | Expanded View |

 And grouping relationships can be depicted using a box to group the elements.

| **Ontology Relationship**                   | **Source**  | **Target**  | **Depiction** |
| ------------------------------------------- | ----------- | ----------- | ------------- |
| hasTaskGroup (isTaskGroupFor)               | Task        | Task        | Grouping Box  |
| hasAssetGroup (isAssetGroupFor)             | Asset       | Asset       | Grouping Box  |
| hasParticipantGroup (isParticipantGroupFor) | Participant | Participant | Grouping Box  |

1. Visual Language Summary

![Diagram

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-4.png) 

![Diagram

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/diagram-description-automatically-generated-5.png) 

![A picture containing letter

Description automatically generated](https://wordpress-540823-2632485.cloudwaysapps.com/wp-content/uploads/2022/06/a-picture-containing-letter-description-automatic-1.png) 

1. <https://movielabs.com/ontology-for-media-creation/> [↑](#post-2342-footnote-ref-2)
2. “The Evolution of Media Creation,” August 2019, <https://movielabs.com/production-technology/> [↑](#post-2342-footnote-ref-3)
3. This is called a trapezium in British English. We make this note to avoid confusion because a trapezoidal shape with no parallel lines is called a trapezoid in British English and trapezium in America English. [↑](#post-2342-footnote-ref-4)
4. This definition excludes the common use of ‘service’ in the production industry as a term for what a person or organization offers the production, e.g., “craft services.” [↑](#post-2342-footnote-ref-5)
5. That is almost universally true particularly if you consider that programmable logic as running software. [↑](#post-2342-footnote-ref-6)
6. See the Common Security Architecture for Production specification. <https://movielabs.com/production-technology/security/> [↑](#post-2342-footnote-ref-7)
7. Unicast means a message is sent from the sender to a single recipient. Multicast means a message is sent from the sender to a defined group of recipients. Broadcast (not used in the diagram) means a message is sent from a sender to every recipient and is a particular type of multicast. [↑](#post-2342-footnote-ref-8)
8. We tried hard to find the name for a shape of this type but have been unable to find one! [↑](#post-2342-footnote-ref-9)
