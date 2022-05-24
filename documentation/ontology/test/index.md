---
version: v..
key: 
id: 
slug: 
weight: 

---
Converting Microsoft Word documents to Markdown user Guide Contents [1 Introduction 2][1] [2 Assumptions 3][2] [3 Conversion Tools 4][3] [3.1 Software Tools 4][4] [4 Setting Up Working Directories 5][5] [5 Conversion Steps 7][6] [6 Editing Markdown Files 10][7] [7 Checking in Documents and Making Pull Requests: 18][8] [8 Conclusion 23][9] **VERSION HISTORY**
<table>
<tbody>
<tr>
<td><strong>Author</strong></td>
<td><strong>Date</strong></td>
<td><strong>Version Notes</strong></td>
</tr>
<tr>
<td>Jake Winett</td>
<td>10/6/2021</td>
<td>First draft</td>
</tr>
<tr>
<td>Jake Winett</td>
<td>10/19/2021</td>
<td>Added naming conventions, folder structure</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
© 2021 Motion Picture Laboratories, Inc.

# <a id="post-603-_Toc84425522"></a>Introduction This document describes the process, challenges, and caveats for converting Microsoft Word files (.docx) created with the MovieLabs documentation template [link] to Markdown (.md) files to display them in an online format on

&lt;https://mc.movielabs.com&gt;.<img class="wp-image-943" src="http://movielabs-api.test/wp-content/uploads/2022/05/a-screenshot-of-a-computer-description-automatica-7.png" alt="A screenshot of a computer Description automatically generated" />

# <a id="post-603-_Toc84425523"></a>Assumptions This document assumes that the user has already installed Git and GitHub on their computer and has appropriate read/write access to the development repository for the documentation website. If not, please contact Damon Boynton (

&lt;dboynton@movielabs.com&gt;) or Daniel Lucas (&lt;dlucas@movielabs.com&gt;) to get this software installed and access established.

# <a id="post-603-_Toc84425524"></a>Conversion Tools Conversion requires the use of some software tools. These are the tools used at the time this document was created. Note that a software license may be required beyond the initial trial period for this software. These tools run exclusively on Windows 10 or higher. macOS users may need to install

[BootCamp][10] or [Parallels][11] to run a version of Windows on their Mac machine. Parallels allows you to switch easily between macOS and Windows without rebooting, but either solution will work.

## <a id="post-603-_Toc84425525"></a>Software Tools

* Writage (&lt;https://www.writage.com&gt;) Markdown plugin for Microsoft Word (macOS or Windows). This plugin allows you to export .md files from Microsoft Word.
* Markdown Monster (&lt;https://markdownmonster.west-wind.com/download&gt; ). Markdown editor software for viewing, editing, and pushing .md files to the repository. (Windows only).
* GitHub Desktop (&lt;https://desktop.github.com&gt; ) – Required to manage your local site code repository, as well as Pull Requests for committing Markdown files to the Git repo.

## Templates Authors should use one or more of the following templates for creating documents that will appear online and/or be made available as a PDF download:

* Use [this template][12] for creating documents in Word intended to be converted to a downloadable PDF. An accompanying **template user guide** can be found [here.][13]

# <a id="post-603-_Toc84425526"></a>Setting Up Working Directories Before beginning, you need to set up a default directory on your machine (or on OneDrive) to save and edit the versions of Word and Markdown files that need to be converted. It is suggested that this has a logical folder structure that follows the categories and sections of the documents themselves. Here is an example of a directory structure created in OneDrive for the Ontology documentation:

<img class="wp-image-944" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-email-35.png" alt="Graphical user interface, text, application, email Description automatically generated" /> Additionally, you will want to set up your default GitHub directories where finished markdown files will be saved and pushed to the repository. Again, this should follow a logical structure according to the content topics and sections. Here is an example of my GitHub working directories:<img class="wp-image-945" src="http://movielabs-api.test/wp-content/uploads/2022/05/a-picture-containing-graphical-user-interface-des-14.png" alt="A picture containing graphical user interface Description automatically generated" />

# <a id="post-603-_Toc84425527"></a>Conversion Steps The following basic steps are required to convert most MovieLabs Word documents into Markdown. Please ensure you are working with the most recently published/released version of the document, which should have an “RC[#]” in the filename.

1. **Open the document:** In Teams, navigate to the folder containing the Word document that needs to be converted, and open the document in the desktop Word application.
2. **Save As:** Immediately do a Save As on the document to your working directory (see above). The naming convention is not critical, but it does make it easier if you follow the convention, “[name]-all.”
1. Example: “**ML\_Ontology\_Pt1\_Overview\_v1.0_RC2.docx**” is Saved As “**overview-all.docx**” into the new directory /Documents/Markdown/Ontology/Overview/.
3. **Hide Markup:** With the copy of the document still open in Word, go to the Review tab, and change from viewing “All Markup” to “No Markup” to hide any remaining comments or redlines in the document.

<img class="wp-image-946" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-338.png" />

1. **Remove Title, TOC, and legal text:** Markdown does not have the means to do a TOC, online navigation is controlled through a combination of the directory/file structure and frontmatter. Therefore, the title header and table of contents should be removed. Also, the legal disclaimer does not need to be in every document, so everything before the first numbered section of the document can be removed. Save the document again, **making sure you are still editing the working copy, not the original.**

<img class="wp-image-947" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-word-14.png" alt="Graphical user interface, text, application, Word Description automatically generated" />

1. **Export file in Markdown:** In Word, select File/Save a Copy, and in the File Format menu, select “Markdown (*.md).” Save the document in the current working directory or another directory if desired. Keep the filename as “[topic]-all.”<img class="wp-image-948" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-email-36.png" alt="Graphical user interface, text, application, email Description automatically generated" />
2. **Ensure you have two files:** You should have two copies of the document in the working directory – one .docx file and one .md file. Close the file in Word and proceed to the next step.

<img class="wp-image-949" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-teams-7.png" alt="Graphical user interface, text, application, Teams Description automatically generated" />

# <a id="post-603-_Toc84425528"></a>Editing Markdown Files

**1. Open the Markdown Monster application.** You may also want to create a file association between .md files and Markdown Monster, which will make them easier to open from File Explorer in the future. Navigate to the directory where you saved the .md file in Step 6 and double-click to open it. You may need to adjust the application pane widths to see the Markdown and Preview correctly.<img class="wp-image-950" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-49.png" alt="Graphical user interface, text, application Description automatically generated" />

1. **Save the document as separate markdown files:** The next step is to break the document into individual files, usually separating into sections denoted by Heading 1 titles in the document. For example, the [**Ontology Overview**][14] document would break into the following sections:
1. Need for an Ontology
2. What This Ontology Covers
3. Technical Notes
4. Documentation
5. Future Expansion This can be accomplished in a few ways – the most straightforward way is to create a new, blank markdown document in Markdown Monster (File/New or Ctrl+N) and

**save it to the current working GitHub directory** (see Section 2 Assumptions) using the topic and section as the filename – (example: “overview-need.md”). Then copy everything from “Need for an Ontology up until “What This Ontology Covers” and paste it into the new document, “overview-need.md” in Markdown Monster. Save the new document again and repeat this process until all the sections have been created as a unique markdown file, following the same naming convention “[topic]-[section].md.” You can leave each section document open in Markdown Monster, making it easier to perform the next few steps.<img class="wp-image-951" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-50.png" alt="Graphical user interface, text, application Description automatically generated" />

1. **Add “Front Matter:”** Each markdown document must have “front matter”. This is metadata used by the website to determine things like the slug (URL) and ordering in navigation menus. This will vary a bit from document to document, but it generally contains these parts:
* 1. **key –** sets what root directory or section the document lives under
2. **id: -** unique name for the document
3. **slug: -** URL directory structure of the document
4. **title:** - The displayed title of the document
5. **weight:** - Display order of the document (lower numbers indicate higher display position).
6. **Pdf:** - Name for associated PDF document (if applicable)
7. **pdfLink:** - filename of linked PDF in the same relative directory (if applicable).
8. ‘\---’: These dashes deliniate the front matter from the document
1. Example and Syntax: \--- key: "documentation" id: "overview-need" slug: "/docs/omc/overview/need" title: "Introduction" weight: 1 pdf: "Media Creation: Overview" pdfLink: "OMC-Overview.pdf" \---

<img class="wp-image-952" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-51.png" alt="Graphical user interface, text, application Description automatically generated" />

1. **Edit Section Heading and Subheadings:** You will likely need to edit the Heading 1 and Heading 2 of each document section. This should mirror the offline document but also make use of the documentation website navigation structure, which will build page contents from Headings 1 thru Headings 4.

**Heading 1:** Use “# ” and then the section heading, e.g., “# Part 1 - Overview.” **Heading 2:** Use “## ” and then the subsection heading, e.g., “## Introduction.”<img class="wp-image-953" src="http://movielabs-api.test/wp-content/uploads/2022/05/text-letter-description-automatically-generated-28.png" alt="Text, letter Description automatically generated" /><img class="wp-image-954" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-339.png" /><img class="wp-image-955" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-340.png" /> This will need to be done for each document section and should coincide with the title used in the front matter of each markdown document.<img class="wp-image-956" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-email-37.png" alt="Graphical user interface, text, application, email Description automatically generated" /><img class="wp-image-957" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-341.png" /><img class="wp-image-958" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-342.png" />

1. **Resolving Conversion Issues:** The Word template translates to Markdown reasonably well, but there are consistent formatting issues that need to be corrected before publishing the markdown documents.
1. Corrections Needed:
1. Term definitions -&gt; Quote Blocks
2. Notes -&gt; needs some HTML formatting
3. Footnotes -&gt; requires renumbering
4. Table Headings -&gt; Change to Italics when needed
2. **Term Definitions to Quote Blocks**
1. **Unedited** Markdown Displayed

**<img class="wp-image-959" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-343.png" />**<img class="wp-image-960" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-344.png" />

* 1. **Edited** Markdown Displayed

<img class="wp-image-961" src="http://movielabs-api.test/wp-content/uploads/2022/05/logo-company-name-description-automatically-gene-7.png" alt="Logo, company name Description automatically generated" /><img class="wp-image-962" src="http://movielabs-api.test/wp-content/uploads/2022/05/a-picture-containing-graphical-user-interface-des-15.png" alt="A picture containing graphical user interface Description automatically generated" /><img class="wp-image-963" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-345.png" />

1. **Notes HTML Formatting**
1. **Unedited**

<img class="wp-image-964" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-application-teams-desc-7.png" alt="Graphical user interface, application, Teams Description automatically generated" /><img class="wp-image-965" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-346.png" /><img class="wp-image-966" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-347.png" /><img class="wp-image-967" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-348.png" /><img class="wp-image-968" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-349.png" /><img class="wp-image-969" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-350.png" /><img class="wp-image-970" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-351.png" />

* 1. **Edited**

<img class="wp-image-971" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-email-38.png" alt="Graphical user interface, text, application, email Description automatically generated" /><img class="wp-image-972" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-52.png" alt="Graphical user interface, text, application Description automatically generated" /><img class="wp-image-973" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-352.png" /><img class="wp-image-974" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-353.png" /><img class="wp-image-975" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-354.png" /><img class="wp-image-976" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-355.png" />

* 1. **Footnote Renumbering:** In the Word/PDF documents, footnotes are in sequence since it is just a single document. When you break up the documents into separate markdown sections, the footnote numbering will restart at “1”. If you would like to edit the footnote numbering to be sequential throughout the entirety of the document (including all sections) then you will need to go the second/third sections, et al, and manually change the numeric sequence.
2. Footnotes are identified by “[^[number]] “ (e.g. “[^2]”). They must be changed in two places – once in the paragraph and once for the corresponding footnote. See Example:

<img class="wp-image-977" src="http://movielabs-api.test/wp-content/uploads/2022/05/text-letter-description-automatically-generated-29.png" alt="Text, letter Description automatically generated" /><img class="wp-image-978" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-356.png" /><img class="wp-image-979" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-357.png" />

1. **Table Headings Use Heading 5:** Depending on the document, the author, and the template, table headings are not consistently formatted to use Italics. You should do a scrub of each table to make sure the heading is formatted correctly:
1. **Incorrect:**

<img class="wp-image-980" src="http://movielabs-api.test/wp-content/uploads/2022/05/text-letter-description-automatically-generated-30.png" alt="Text, letter Description automatically generated" /><img class="wp-image-981" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-358.png" />

* 1. **Correct:**

<img class="wp-image-982" src="http://movielabs-api.test/wp-content/uploads/2022/05/text-letter-description-automatically-generated-31.png" alt="Text, letter Description automatically generated" /><img class="wp-image-983" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-359.png" />

1. **Add Images:** Some documents will have embedded images in the Word/PDF versions. These images will need to be extracted and placed in a source folder referenced in the markdown document as a relative path.

<img class="wp-image-984" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-application-website-de-7.png" alt="Graphical user interface, application, website Description automatically generated" /> In Markdown, this image would be referenced in the following way:<img class="wp-image-985" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-360.png" /> Note: In the Markdown Monster preview pane, the image may appear as a broken image link.

1. **Fix Cropped Powerpoint images:** Writage consistently messes up cropped powerpoint images and adds in the full slide instead of the cropped image. Writage notes this by giving the image a name that says the image was dynamically created. Go to Word version and save out figures as pictures. Usually good idea to just save them with the figure name into the image folder.

# <a id="post-603-_Toc84425529"></a>Checking in Documents and Making Pull Requests: Once Markdown documents have been converted and corrected, they can be pushed to the Git repository and pulled into the CI/CD process for building the site.

1. **Save Documents:** In Markdown Monster, make sure that you have saved each document to its folder, which is designated as the Git folders on your local machine (the folder could be a cloud/OneDrive folder as well, but just needs to be mounted and accessible from File Explorer). Note that documents with unsaved changes will have a “*” in the document name tab.

<img class="wp-image-986" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-word-15.png" alt="Graphical user interface, text, application, Word Description automatically generated" /><img class="wp-image-987" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-361.png" />

1. **Open GitHub:** (Depending on your familiarity or comfort using Git/GitHub, some may prefer using the command line interface for Git, but only the desktop app is referred to in this document).
2. **Fetch Origin:** If you haven’t opened GitHub recently, perform an origin refresh to ensure you have the latest repo updated on your local machine. Also, make sure that the current branch is set to “Dev.” (note: this is the correct setting as of the writing of this document, but it might be preferable later to have people only working in their own dev branch vs. writing to the main branch).

<img class="wp-image-988" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-53.png" alt="Graphical user interface, text, application Description automatically generated" /><img class="wp-image-989" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-362.png" /><img class="wp-image-990" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-363.png" />

1. **Create “Local” Branch:** If ‘local’ exists and isn’t identical to ‘dev’, use local-[gitUsername] instead. (note: if you’re not sure if ‘local’ is identical to ‘dev’, use local-[gitUsername])
2. **Verify Changed Files:** After saving files in Markdown Monster, they should appear in GitHub under the Changes tab. Confirm that all of the new files or changes appear as expected.

<img class="wp-image-991" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-54.png" alt="Graphical user interface, text, application Description automatically generated" /><img class="wp-image-992" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-364.png" /><img class="wp-image-993" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-365.png" />

1. **Add Update Notes:** If you are updating multiple files, you will need to add a title as well as a description of what has been updated. The title and description should be brief but descriptive enough to inform someone else about what changes were made. Some examples:
1. “Corrected Notes formatting issues.”
2. “Made change to front matter.”

<img class="wp-image-994" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-descr-55.png" alt="Graphical user interface, text, application Description automatically generated" /><img class="wp-image-995" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-366.png" /><img class="wp-image-996" src="http://movielabs-api.test/wp-content/uploads/2022/05/word-image-367.png" />

1. **Commit Changes to Current Branch:** Click the “Commit to [currentBranch]” button to commit these changes to the repo.
1. There is the potential for conflicts if two people are making changes to the same document. If this is the case, you should contact the other developer (e.g., Daniel) to confirm whether you should overwrite those changes or wait to refresh the origin and commit your changes later.
2. **Create Pull Request:** Create pull request into ‘dev’
3. **Resolve Pull Request:** Go to github website and resolve the pull request. If you don’t know how to do this, contact [Damon Boynton][15] or [Daniel Lucus][16] for instructions.
4. **Verify Changes in Dev Build:** Once you have made the commit, wait 5-10 minutes before going to &lt;https://develop-mc.movielabs.com&gt; to manually validate the changes were made. If the site isn’t updated after 10 minutes, contact [Daniel Lucus][16] to confirm that the CI/CD process is still working as expected.

<img class="wp-image-997" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-description-automa-7.png" alt="Graphical user interface, text Description automatically generated" />

# <a id="post-603-_Toc84425530"></a>Authoring and Naming Files Documentation will also be made available for download as standalone PDF files.

## Document File Naming

* Applies to Word, Excel, PDF, PowerPoint, ZIP files, et al.
* File names should use dashes (“-”) to separate words, and not use underscores, spaces, or other characters.
* **Good** Example: **ML-Ontology-Pt1-Overview-v.1.0.docx**
* **Bad** Example: **ML\_Ontology Part 1 Overview v\_1.0.docx**

## Versioning

* Version numbers should be at the end of the file name and reflect the version number of the most recently published document.

## Authoring/Packaging When creating a ZIP file containing multiple files, use a logical directory structure that will be copied to the user’s computer when they download and unzip the file.

**For the ZIP file “ML-Visual-Language-v1.0.zip”**<img class="wp-image-998" src="http://movielabs-api.test/wp-content/uploads/2022/05/graphical-user-interface-text-application-email-39.png" alt="Graphical user interface, text, application, email Description automatically generated" />

## Image Folder Pathing Images are separated out into a media file when a docx is converted to markdown. They need to be transferred to the static file folder in the Website git hub in order to work. Since this requires a

# Conclusion This is the basic process for converting Word documentation to Markdown for the MovieLabs Documentation website. Please continue updating this document as processes evolve and change.

[1]: #post-603-_Toc84425522
[2]: #post-603-_Toc84425523
[3]: #post-603-_Toc84425524
[4]: #post-603-_Toc84425525
[5]: #post-603-_Toc84425526
[6]: #post-603-_Toc84425527
[7]: #post-603-_Toc84425528
[8]: #post-603-_Toc84425529
[9]: #post-603-_Toc84425530
[10]: https://support.apple.com/boot-camp
[11]: https://www.parallels.com/products/desktop/trial/
[12]: https://movielabs.sharepoint.com/:w:/s/internalproductiontechnologypm/Ef8ii-gKMLhHmFr82Ja1JQYBCiOpPlwS_MeF3uugzxUSLw?e=6OMatr
[13]: https://movielabs.sharepoint.com/:b:/s/internalproductiontechnologypm/Eff4gme4yGpKv62TORBMjNsBGt4RrlCkdP_13fpjsfL2yA?e=9BdMGM
[14]: https://teams.microsoft.com/l/file/CCCC97A4-D8BE-42AC-8863-2111C2C1C367?tenantId=883197d1-18e1-40b8-af69-90d9b766f7f3&amp;fileType=docx&amp;objectUrl=https%3A%2F%2Fmovielabs.sharepoint.com%2Fsites%2Fcloudproduction%2FShared%20Documents%2FGeneral%2FPartner%20Previews%2FML_Ontology_Pt1_Overview_v1.0_RC2.docx&amp;baseUrl=https%3A%2F%2Fmovielabs.sharepoint.com%2Fsites%2Fcloudproduction&amp;serviceName=teams&amp;threadId=19:41a9950ceff04518a25d97f857c0cc0d@thread.tacv2&amp;groupId=5192d19a-d903-4fd0-a7e4-ef2c36a32b6e
[15]: mailto:dboynton@movielabs.com?subject=Movielabs%20Website
[16]: mailto:dlucas@movielabs.com?subject=Movielabs%20Website