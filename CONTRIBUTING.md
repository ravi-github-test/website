# Contributing

We welcome and value contributions from everyone. 

## Contribution Types

Below are some ways in which you can help. 

- Code contributions (typo fixes, website enhancements, improving documentation, etc.)
- Design contributions (e.g. graphic design for the website and/or social media)
- Cloud/Infrastructure Sponsorship - Having cloud/infrastructure resources would help lower the barrier for us to add more functionality to our website. If you are interested in supporting the JEDI Outreach Group by providing such resources, please contact us at admin@datascijedi.org. 
- Website expertise - If you're knowledgable about website development (e.g. creating the backend for a website application), we would be interested in hearing your ideas (whether you can provide development time or not). Please get in touch at admin@datascijedi.org. 
- Any other ideas? Feel free to open a Github issue to suggest and discuss ideas, or get in touch with us at admin@datascijedi.org. 

## Workflow for Code Contributions

For code contributions, please submit a PR using the following steps:

1) Clone (or fork, for new contributors) the [datascijedi/website](https://github.com/datascijedi/website) repository. 
2) Create a branch using a descriptive name (e.g. `my-awesome-feature`) and make your additions there. 
3) Create a pull request from `my-awesome-branch` in your cloned (or forked) repository to the `main` branch of the [datascijedi/website](https://github.com/datascijedi/website) repository. 

In addition, consider creating a relevant GiHub issue so that other contributors are aware and can comment on your proposed work, especially if your work is a larger effort that may take some time to complete. 

## Local Dev Setup

We use the Quarto framework for website development. Below are some steps to get up and running:

1) Download and install Quarto from [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/). 
2) Fork and clone this repository. 
3) Navigate to the root of the cloned repository and run `quarto preview`. This should open up a local version of this website in your browser. 

There are various ways to develop using Quarto, so feel free to check out the official [Quarto docs](https://quarto.org/docs/get-started/hello/) for more information. 

## Adding links
When inserting links anywhere on the site, use clear label describing the purpose of the link. This makes the website more accessible for viewers using screen readers (among other accecsibility benefits). [Read more about Accesible Rich Interner Applications at this link.](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA8#:~:text=The%20aria%2Dlabel%20attribute%20provides,used%20instead%20of%20aria%2Dlabel%20)

## Updating Resources
For adding links to Resources tab, open the resources.qmd file (in the "main" folder). Click the pencil icon to edit the file. Copy the formatting for other links, that is putting the text description within brackets and website within parentheses. Leave a vertical space between each bullet point resource. Commit changes to save. 

## Updating Webinars

### Upcoming webinars

For adding information on upcoming webinars, use the following stpes:

1) Add webinar image or flyer to website/webinars/images. Note, pdf flyers are not ideal; they don't display well. png or jpg are preferred.
2) Copy content of dummy-webinar.qmd from website/webinars
3) Create new .qmd file in website/webinars/upcoming, paste dummy-webinar content, and edit all available fields.
4) If necessary, update website/webinars.qmd to replace "Coming soon" message, display upcoming webinars. Use <!-- at the start of Coming soon message and --> at end to supress. Remove #s on listing content to show upcoming webinars (lines 4-8). (Ensure proper spacing, look at past webinars list for example.) Remove <!-- and --> around :::{#upcoming webinars} ::: 
5) If necessary, update index.qmd to display upcoming webinars instead of past webinars. To do this, change content from webinars/past to webinars/upcoming
 
 ### Past webinars
 
 When a webinar has occurred, use the following steps to move it to past webinar list, update home page, and remove it from upcoming webinar page:
 
 1) Copy template from a past webinar (in website/webinars/past/)
 2) In website/webinars/past folder, click Add file and select Create new file.
 3) Name file used date and topic and .qmd file type (e.g., 2023-01-20-disabilities-transitioning.qmd)
 4) Paste copied template
 5) Edit template with webinar specific information. (Can open github in a separate tab to copy information.)
 6) When/if webinar video and slides are available, add links under Recording and SLides. If not available, use "<!--" to suppress these lines of code. Can leave note: "Recording coming soon. Sign up for our [weekly newsletter](weekly-newsletter.qmd) to be notified when recording is available." 
 7) Commit new file
 8) IF THERE ARE NO UPCOMING WEBINARS, update website/webinars.qmd. with the follow: comment out upcoming webinars on the listing (from - id: upcoming webinars to type:default); use "<!-- ... -->" to suppress upcoming-webinars and remove these from around "New webinars are coming" message. 
 9) IF THERE ARE NO UPCOMING WEBINARS, update index.qmd to display past webinars instead of upcoming. To do this, change content from webinars/past to webinars/upcoming. (Home page may look the same since this webinar will still be featured, but check that link goes to past webinar page instead of page.) 
 10) Delete page from website/webinars/upcoming.

