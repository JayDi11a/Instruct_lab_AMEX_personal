Spike \- Process Article Template Model (WatsonX)
This document outlines a working template model for Process Articles that can be used when uplifting existing TZ (ECCO) content into a POA format.
When generating an output for process articles, the following writer's guides must also be followed to adjust aspects of the article such as, wording
/language, formatting, restructuring, validations etc.
https://thesquare.americanexpress.com/sites/business\-unit/global\-services\-group/global\-stra\[…]business\-partners/documents/756371/chc\-a\-z\-style\-guide
https://thesquare.americanexpress.com/sites/business\-unit/global\-services\-group/global\-stra\[…]ledge\-management/documents/655385/process\-author\-
guide
Key Details
Facts about Content Shared To\-Date
Assumptions
Process Article Template
Title
Overview
Sections
Template Example
Key Details
Facts about Content Shared To\-Date
The content being shared with IBM for AI experimentation is an extract from the KML CMS's API called 'Natural\-Text\-API'. During extraction, this performs
some cleanup and adjustments to the ECCO content upfront.
Specifically:
Removal of any unsupported html tags that do not fall into the category of 'content' (tags \& attributes used for styling, scripts for interaction etc).
Automatic formatting of Acronyms to current GKLM standard when detecting acronyms defined according to ECCO's writer's guideline.
Automatic insertion of heading tags (where appropriate) to enable ECCO content to comply with the natural\-text\-api contract.
Assumptions
The extract from the API is a better baseline than the unadjusted raw output from the CMS
The raw output is JSON format with html contained within the value of the keys.
The adjusted output is more AI friendly as it uses a consistent format, reducing the need for bespoke instructions to work around the
content model.
Output from this POC is produced using a template that enables compatibility for storing this content using our existing Structured\-Content\-
Model.
Structured model allows us to deliver the same content to many downstream channels today.
Where each consuming system decides on visualisation or other requirements using the information provided by the structure.
Output from this POC is an approximation of a template that GKLM may define for content intake process.
There is no format template in use today for Process Articles.
We should base target template using the POA Process Article Model defined in natural\-text\-api.
This accelerates KA compatibility and allows testing and fine\-tuning without the CMS complexity.
Proven to work well with LLM already.
The template will not be a 1:1 with this API, but rather a version from this that is more akin to what a GKLM intake process template may
look like.
Not necessarily tied to the CMS's content model.
The expected output should only consist of Process related content.
ECCO Process Articles sometimes are split into multiple Articles if different types when GKLM manually uplift the content.
For the purpose of this POC, we may uplift all content as Process to begin with for simplicity.
Therefore, the template only defines minimum requirements for a Process Article.
Process Article Template
At a high level, a process article is composed of the following structure:
Title
Overview
Sections
Additional Information \- Not in scope
Revision History \- Mapping not
required
Metadata \- Not in scope
Title

Must use tag

H1 is reserved for this field only and must not be used anywhere else in the document. Title
must be less than 5000 characters long.
Overview
Must use  tag.
Must use the word 'Overview', translated according to the language of the article.
Content in overview can use rich text using following safe list:
Allowed Tags: p, strong, em, u, li, ul, ol, a, h3, h4, h5, h6, pre, address
Allowed attributes for tags:
a \- href, target, data\-type, title, id
p \- style
Sections
A series of 'context sections', where each section must include a section title, where the title must be surrounded by  tag.
Each section's title is required to use  to maintain uniformity across the document. A section can be categorised into one
of the following, where each has specific requirements:
A general section
Allowed Tags: p, strong, em, u, li, ul, ol, a, h3, h4, h5, h6, pre, address, table, thead, tbody, tr, th, td
Allowed attributes for tags:
a \- href, target, data\-type, title, id
p \- style
th \- scope
Images must be defined according to the following structure:
title of the image using  tag
optional description using the same allowed tags as per article's overview
alt text must be provided within a single  tag enclosure with all inner content in plain text
link to image must be provided as an S3 reference path under a single * tag enclosure
A Step\-by\-Step section
Optionally include an overview, which follows the same safe list as the main overview of the article.
Each Step must be defined using  tag.
Each Step must be labeled as 'Step 1', 'Step 2' etc, with localisation according to the language of the article.
Each Step's content can be defined accordingly:
Allowed tags: p, strong, em, u, li, ul, ol, h4, h5, h6, pre, address, table, thead, tbody, tr, th, td
Allowed attributes for tags:
a \- href, target, data\-type, title, id
p \- style
th \- scope
Images must be defined according to the following structure:
title of the image using  tag
optional description using the same allowed tags as per article's overview
alt text must be provided within a single  tag enclosure with all inner content in plain text
link to image must be provided as an S3 reference path under a single 
	+ tag enclosure
	An optional section after all step definitions:
	Must use  tag
	Must be labeled 'additional text'
	Follows the same allowed tags as per the article's overview
	A File(s) attachment section
	This section's  title must read 'Attachment(s)', translated according to article's language
	For each file, a title must be defined using  tag
	An optional description using the same safe list as per article's over link
	teust be provided as an S3 reference path under a single 
		- tag enclosure
		
		Template Example
		A formatted output example of this article looks like the following:
		Title of the article
		Overview
		A brief summarisation of the Article
			* Bullet point 1
			* Bullet point 2Further description
		A general section example
		Example content in this general section
		Example sub section heading
		Sub section content
		
		| Header Column 1 | Header Column 2 |
		| --- | --- |
		| Row 1 Column 1 Cell | Row 1 Column 2 Cell |
		| Row 2 Column 1 Cell | Row 2 Column 2 Cell |
		
		Some further information within this general section
		An image example
		Optional image description using **rich text**
		Alt test that is written in plain text
		
			* /path/to/file/file\-name.png
		An example step\-by\-step section
		Optional overview of the steps section
		More steps overview content
		Step 1
		Ask a question here?
		
		
		| Yes | Go to Step 3 |
		| --- | --- |
		| No | Go to Step 2 |
		
		
		Step 2
		Follow instructions in this step
		Process is complete
		Step 3
		Follow instructions in this step
		An image within a step example
		Optional image description using **rich text**
		Alt test that is written in plain text
		
			* /path/to/file/file\-name\-2\.png
		Process is complete
		additional text
		Optional additional text for this step\-by\-step
		Another section that could be generic or step\-by\-step
		...
		...
		Attachment(s)
		Attachment 1 title
		Optional description of file
		
			* /path/to/file/attachment\-1\.doc
		Attachment 2 title
		
			* /path/to/file/attachment\-2\.doc
