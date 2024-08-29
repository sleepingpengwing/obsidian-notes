Traditional web applications - browser fetches HTML Doc 
	Either static or dynamic - simple text file within directory or based on applications code
const getFrontPageHtml = noteCount => {
  return `
    <!DOCTYPE html>
    <html>
      <head>
      </head>
      <body>
        <div class='container'>
          <h1>Full stack example app</h1>
          <p>number of notes created ${noteCount}</p>
          <a href='/notes'>notes</a>
          <img src='kuva.png' width='200' />
        </div>
      </body>
    </html>
`
}

app.get('/', (req, res) => {
  const page = getFrontPageHtml(notes.length)
  res.send(page)
})
Example of code formed dynamically^

ul-tag - unordered list
Keep tabs on Console tab and the console.log command

Events handlers and callback functions
	Basically rules/function set in place once variable is reached based on browser/environment
Document Object Model (DOM)
	API that modifies the elements trees of webpages
	EX) variable ul from earlier being a "branch"

![[Pasted image 20240828201717.png]]
Evidence of actually hacking the mainframe of this dumb website^

CSS
	Cascading Style Sheets - determines webpage appearance
	.notes - always starts with . and contains the name of class/attribute (notes, container, etc)
	could modify "rules" (border size, color, etc)

Loading page REVIEW
	![[Pasted image 20240828202755.png]]
Forms and HTTP POST
	Form element - allows users to submit/enter data, which is then sent and event that does blah blah
	In the case of this website, the "new note" is the data sent as the body of the POST 
AJAX (First Descendent)
	Asynchronous JavaScript and XML - enabled data fetch of content using Java within the HTML, with no need to rerender
Single page app (SPA)
	Diff from trad. - only one HTML page
JavaScript-libraries
	