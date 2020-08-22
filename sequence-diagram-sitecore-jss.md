sequenceDiagram
	Client-->>Node Server: request to a site url.
	Node Server-->>Sitecore: request page and layout information.
	Sitecore-->>Node Server: return layout data.
	Node Server-->>Sitecore: request item data based off of layout information.
	Sitecore-->>Node Server: return item data.
	Node Server-->>Node Server: render the page component with data.
	Node Server-->>Sitecore: request item data based off of layout information.
	Sitecore-->>Node Server: return item data.
	Node Server-->>Node Server: render the page component with data.
	Node Server-->>Client: return fully rendered page.

	
					