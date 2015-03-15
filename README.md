# A.Accordion
A simple Bootstrap accordion menu with toggle icon.

[Checkout the demo](http://wjpdesigner.com/aaccordion/)

[![Image of ACarousel](http://wjpdesigner.com/aaccordion/screenshot.jpg?1)](http://wjpdesigner.com/aaccordion/)

### Feature:
- Fully Responsive
- Minimalist Design
- Easy to use just 3 steps

### Implementation:
#### 1.Getting Started
Load Bootstrap and AAccordion files.
```html
<!--Bootstrap CDNs-->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
<script src='https://code.jquery.com/jquery-1.11.2.min.js'></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>
<!--AAccordion CSS-->
<link rel="stylesheet" href="aaccordion.css">
```
#### 2.Set up your HTML
Inside the container `.panel-group` you can add as many as panels as you want. But make sure that `href="#xxxOne"` matching with panel `id="xxxOne"`.
```html
<!--START Accordion--><div class="panel-group" id="accordion">
	
		<!--START Panel One-->
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class="panel-title">
					<a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapseOne">
						CREATIVE MARKETING AND COMMUNICATIONS
					</a>
				</h4>
			</div>
			<div id="collapseOne" class="panel-collapse collapse">
				<div class="panel-body">
					<p>Creative Marketing and Communications focuses on the development and execution of communication initiatives that convey the Coach brand image and positioning. Creative Services is our internal creative agency that designs, develops, and produces global advertising and marketing collateral. Press Relations plans and executes innovative communication strategies including editorial coverage with global fashion media and brand-enhancing events to elevate Coach’s brand cachet.</p>
					<a href="https://www.coach.apply2jobs.com/ProfExt/index.cfm?fuseaction=mExternal.showSearchInterface" target="_blank">see current jobs</a>
				</div>
			</div>
		</div>
		<!--END Panel One-->
		
		<!--START Panel Two-->
		<div class="panel panel-default">
			<div class="panel-heading">
				<h4 class="panel-title">
					<a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapseTwo">
						CUSTOMER EXPERIENCE
					</a>
				</h4>
			</div>
			<div id="collapseTwo" class="panel-collapse collapse">
				<div class="panel-body">
					<p>Our Customer Experience team ensures Coach delivers best-in-class service and seamless experiences consistently across all global consumer touch points—in store, online, and within our call centers. Through a deep understanding of our customers and their preferences around the world, the team defines and refines Coach’s customer experience standards and delivers the capabilities, processes, technology, and metrics to drive and measure results.</p>
					<a href="https://www.coach.apply2jobs.com/ProfExt/index.cfm?fuseaction=mExternal.showSearchInterface" target="_blank">see current jobs</a>
				</div>
			</div>
		</div>
		<!--END Panel Two-->
		
<!--END Accordion--></div>	
```
#### 3.Style your accordion in CSS
```html
.panel-heading .accordion-toggle:after {
    content: "\2212"; /*Adding the toggle icon here*/
	font-size: 20px;
	font-weight: normal;
    float: right;
	margin-top: -2px;
}
.panel-heading .accordion-toggle.collapsed:after {
    content: "\002B"; /*Adding the toggle icon here*/
	font-size: 20px;
	font-weight: normal;
}
```
### Copyright and License:
The MIT License (MIT)

Copyright (c) 2015 wjpdesigner.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.