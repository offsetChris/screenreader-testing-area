# Screenreader testing site

In partnership with the manual testing group this is a place to test common HTML and CSS structure with screenreader and browser combinations. 

## Site is hosted here: on [GithubPages](https://offsetchris.github.io/screenreader-testing-area/)

## Future considerations:
	* Recording findings for all HTML/CSS examples and browser/screenreader combinations. Writing out what the screen reader states for each. 
	* Add more examples of alternative structures or implementations. <section> vs role="region". Aria-label with title and html text in same element etc. 
	* Graph out usage per population pulling in webaim's data for screen reader usage. 
	* Adding more complex interaction and CSS display properties to test with assistive tech. 

[ ] Breadcrumb links
[ ] equivalent HTML markup for landmarks doesn't allow traveling by region. NVDA specific example for hotkeys. (What browsers/screen readers do not allow for hotkey travel?)
[ ] todo: look up if heading can have nested anchor. Also if anchor have nested heading which pretty sure is not allowed but detail that out
[ ] Add examples without "navigation" in the aria label value. 
[ ] HTML5 semantic tabs <header>, 
[ ] when do HTML landmarks need roles and when does HTML5 work for semantics. 
[ ] Form labeling. 
[ ] img tag with role=img
[ ] banner put text on a picture and did the background correctly - div role="img" with aria label and html text inside div. 
[ ] How does tabindex forcing on a div with aria label change the results. 
[ ] 



## results
JAWS chrome conveys nav as navigation region
JAWS chrom did not read aria-label on a div alone you must use role="navigation" to ensure it is read. 
JAWS chrome did not read duplicate information for nav with role="navigation"
Jaws chrome read duplicate info with nav and aria-label even thou

NVDA results were identical, 

Voiceover
mostly the same

Interesting things:
Jaws/chrome and voiceover tells user when navigation ends. 
NVDA and voiceover convey when region ends
The footer tag was never read by any pairing
The nav with aria label was the only duplicate information. 


