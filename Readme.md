# T1A2 Portfolio  

# URL to website:
	- https://gysohn.com/

# Link to your GitHub repo:
	- https://github.com/gysagsohn/gysohn_T1A2

# Link to presentation video of the website:
https://youtu.be/7OWuIzKu_V8

# Layout/responsive layout
Using Figma I have set the limits of the size as per below:
    -desktop 1280 X 800
    -tablet 1020 x 950
    - mobile phone 300 x 700


# I started the project by using Figma to create the layout for my website: 
# Version 1:
	About page
	/gysohn_T1A2/docs/webpage_layout/V1.0/About_page/mobile_about.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/About_page/tablet_about.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/About_page/desktop_about.png

	Index/home
	/gysohn_T1A2/docs/webpage_layout/V1.0/Home_page/desktop_home.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Home_page/HOME_PHONE.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Home_page/tablet_home.png

	Blog
	/gysohn_T1A2/docs/webpage_layout/V1.0/Blog_page/desktop_blog_opt1.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Blog_page/desktop_blog_opt2.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Blog_page/tablet_blog.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Blog_page/tablet_mobile.png
	- for the blog page two designs was considered originally for desktop

	Contact
	/gysohn_T1A2/docs/webpage_layout/V1.0/Contact_page/desktop_contact.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Contact_page/mobile_contact.png
	/gysohn_T1A2/docs/webpage_layout/V1.0/Contact_page/tablet_contact.png


# Purpose:
The purpose of the website was to create and publish a website as a portfolio to demonstrate my skills as a dev and IT skill. Especially to reflect the skills I learnt at Corder Academy so far. My intention was to show case an online portfolio about me, in the areas of skills, interests, professional knowledge and showcase my work. Also, it was to test the skills I have learnt over a short period for time at Corder Academy. 

# Functionality / features
I want to create the following functionality/features
**flex box**
- use flex box to create a responsible website that was visible on multiple different screen size.
- header - flex boxed so that it changes as the screen changes 
- footer - the amount of space the icons take 
- home, blog, contact, about main section - flex boxed so that it changes as the screen changes 
- multiple page that link - create a website with at least 4 pages that are linked and have the similar theme. For the blog page, option 2 was taken as I believed it would have been too similar to other pages if I went with option 1. I wanted to show off a different skill set. About page layout changed from the original plan for the same reason. For the contact page, if I had more time I would have liked to add the social. For detailed breakdown on layout please see below. medial icon to appear next to the contact page and for it to hover/shake at the same time if it was touched. This is explained further in the button section.
- social medial icon - I used an extenal link to creat the icons

```html
	    <!-- Link for fontawesome -->
        <link
            rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
            integrity="sha512-z3gLpd7yknf1YoNbCzqRKc4qyor8gaKU1qmn+CShxbuBusANI9QpRohGBreCFkKxLhei6S9CQXFEbbKuqLg0DA=="
            crossorigin="anonymous"
            referrerpolicy="no-referrer"
            >
```

- icon image - create an icon image and have it showing on webpage

```html
		/gysohn_T1A2/docs/favicon.ico
		 <link rel="icon" href="../images/favicon.ico" type="image/x-icon" >
		/gysohn_T1A2/docs/screenshot_icon.png
```

- nav bar - create a hamburger bar when the screen get smaller. This did not take place as I ran out of time. Instead I created the strike out feature

	```html
		<span class="strike">[page name]</span></a>
	```
	
- buttons - use buttons to link to other pages within the text of the page. Including changing of colour 

	```html
		.contactbutton {
 			background-color: $primary-color;
  			border: none;
  			color: rgb(2, 2, 2);
 			padding: 16px 32px;
  			text-align: center;
  			display: inline-block;
  			font-size: 16px;
  			margin: 4px 2px;
  			transition-duration: 0.4s;
  			border-radius: 30%;
  			cursor: pointer;
			}
   			.contactbutton1 {
    				background-color: $primary-color;
    				color: black; 
    				border: 2px solid #04AA6D;
    				border-radius: 30%;
    				}
    			.contactbutton1:hover {
        			background-color: #04AA6D;
        			color: $primary-color;
    			}

		and spinning
			   .submit:hover {animation: shaking 0.5s infinite;}
        			@keyframes shaking {
            			0% {transform: rotate(0deg);}
            			20% {transform: rotate(-20deg);}
            			50% {transform: rotate(0deg);}
            			70% {transform: rotate(20deg);}
            			100% {transform: rotate(0deg);}
        		}
	```

Using the W3C Markup validation service, I understand that "a must not appear as a descendant of the button element"

```html
	/Users/gysohn/Desktop/Coder_Academy/gysohn_T1A2/docs/W#Cmarkup.png (W3C Markup validation service, no date)
	the code I wrote (1 example as same structure was used for the other buttons):
			<button class="contactbutton contactbutton1">
                            <a href="./contact.html">Contact Me</a>
                        </button>
```	

If I had more time I wish I could have found a solution to this. 
- When opening a link the difference between opening a new tab and continuing. For all external links including the PDF files, additional code of  

		```htm
		target="_blank"
		```

was added to ensure that a new tab opened up

- Hover feature -  adding hovering feature of enlarging to external links

```css
		.social-media:hover {
            		-ms-transform: scale(1.5);
            		-webkit-transform: scale(1.5);
            		transform: scale(1.5);	
```
- home page image
```css
    		.logo-name:hover {
        		-ms-transform: scale(1.5);
        		-webkit-transform: scale(1.5);
       			transform: scale(1.5);
    			}
```

If I had more time I would have limited that to particular size screen only and/or add a different hover feature when the screen size was different
	
# Ensuring all links worked 
- as I didn't have the time to create pages/functions to all the links, such as "read more" and "submit" I create a splash page called "blog2" which has "Watch his space! More to come" with an image. I just wanted to make sure all the links was functional and was linked to a page/action
	
- Blue hyperlink line - I didn't like the blue hyperlink line and changing of colour after clinking. So create a default "noblueline"
		
```css
		a{

    			text-decoration:none;

    		}

			a:link, a:visited {
        			text-decoration: none;
      			}	
```

- colours - to ensure a similar theme over my webpage the following colours were selected and default created:

```css
		$primary-color: #ddf8db;
		$secondary-color: #1238f3;
		$primary-background: #7ebcf1;
		$secondary-background: #7940f4;
```

Please note the above colours were selected as after making the first page, the original colours on the mockup wasn't working for me:
	/Coder_Academy/gysohn_T1A2/docs/firstdraft.jpg


I wish I took more screenshots of my trial and error, as it would have been an easier process to document my decision making process
	
- Font size and colour -
I didn't set one for all the pages, as it made it feel like my first time and I have never been good with design and felt making the decision too hard (especially after what I managed with the colours). However, I did set a font for the webpage to give it a theme through out "font scss"

For size and colour I did make changes as required per section, example below:

```css
	   a {
            i {
                color: rgba(22, 21, 21, 0.664);
                font-size: 50px;
                width: 50px;
            }
	
```
- Breakpoints 
I set the breakpoints based on the the information from Figma:

```css
	$medium: 700px; - tablet
	$small: 310px - phone
	Based on that at certain pages code was added to change layout based on screen size:
	About
	@media screen and (min-width: $small) {
    		main {
    			.content {
        		text-align: justify;
        		padding-right: 40px;
        		padding-left: 40px;
        		}
    		}
	Footer
	@media screen and (min-width: $medium) {
    		footer {
        		.social-media {
            		width: 50%;
            		margin-left: auto;
            		margin-right: auto;
        		}
    		}
	Header
		@media screen and (min-width: $medium) {
    			header {
       			display: flex;
        		align-items: flex-end;
        		justify-content: space-between;

       			 }

        		#nav-items {
            			width: 50%;
        			}
    		}
```

- Layout of main section
I used flex box for all of it, but to test my skills I used different features to achieve the look. Please see examples below:

index/home - flex box with wrap 

```css
			main {
   			display: flex;
    			flex-wrap: wrap;
    			flex-direction: row;
    			justify-content: space-evenly;
    			align-items: center;
  		}
```
	
about - flex box with wrap and row reverse. Just to make it different


```css
			main {
    				display: flex;
    				flex-direction: row-reverse;
    				justify-content: space-evenly;
   				align-items: center;
   				flex-wrap: wrap;
    				gap: 24px;
```

blog - as stated about the below was chosen to make it look different from above. Also, I wanted to create a box to show the image and text as one

			```css
			main {
    				display: flex;
    				justify-content: space-around;
   				align-items: center;
    				flex-wrap: wrap;
   				gap: 24px;

    					article {
        				height: 100%;
       					margin: 20px 0px;
        				border-radius: 8px;
        				overflow: hidden;
        				text-align: center;
        				background-color: $primary-color;
        				border-radius: 20%;
				
						section {
            					.blog-image {
               					width: 300px;
            					}
        				}
    				}
				}
			```

- Blog2 
flex box was not used for the main as it was a simple page and from trial an error it would appear in all screen sizes without issue:

```css
	main {

		.container {
			position: relative;
			text-align: center;
			color: white;
			height: 100%;
		}

			.img {
			width: 100%;
			}

			.centered {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate (-50%, -50%)
			}

	}
```

- Contact
I used flex box to create it. I did try to come up with an idea to make it look different from the style used in class, but I couldn't think of anything better.  I did use different screen sizes to ensure that it would fit on the three different screen sized

```css
		main {
				display: flex;
				flex-direction: column;
				align-items: center;
				margin-bottom: 24px;

				form {

					.form-elements {
							display: flex;
							flex-direction: column;
							margin-bottom: 24px;

						label {
							font-size: 1.2rem;
					}

					.form-input {
					border: 1px solid $primary-color;
					border-radius: 4px;
					outline: none;
					font-size: 1.2rem;

						#form-textarea {
						resize: none;
					}

					&:not(#form-textarea) {
						height: 35px;
					}

					&:focus {
						box-shadow: 0 0 10px 3px $primary-color;
					}

						}
				}

			.submit {
				text-align: center;

					a:link, a:visited,  a:hover, a:active{
					color: #000000;

					}
	
				#submit {
					height: 40px;
					background-color: $primary-color;
					border: none;
					min-width: 120px;
					font-size: 1.2rem;
					border-radius: 30px;
					}
			}


	@media screen and (min-width: $medium) {
			main {
			form {
				width: 500px;

					.form-elements {
					flex-direction: row;
					justify-content: space-between;

						.form-input {
							width: 70%;
						}
					}
			}
			}   
		
```
# Sitemap
# Pages
- Index home https://gysohn.com/
- About https://gysohn.com/pages/about
- Blog https://gysohn.com/pages/blog 
- Blog2 https://gysohn.com/pages/blog2
- Contact https://gysohn.com/pages/contact
- used netlify site map feature. But I am not sure what else to do

Screenshots
- Index home desktop

	/gysohn_T1A2/docs/website_screenshot/index.home/home_index_desktop.png

- Index home tablet

	/gysohn_T1A2/docs/website_screenshot/index.home/home_index_tablet.png

- Index home phone

	gysohn_T1A2/docs/website_screenshot/index.home/home_index_phone.png

- About	desktop

	/gysohn_T1A2/docs/website_screenshot/About/desktop.png

- About tablet

	gysohn_T1A2/docs/website_screenshot/About/tablet.png

- About phone

	/gysohn_T1A2/docs/website_screenshot/About/phone.png

- Blog desktop

	/gysohn_T1A2/docs/website_screenshot/blog /desktop.png

- About tablet

	/gysohn_T1A2/docs/website_screenshot/blog /tablet.png
	
- About phone

	/gysohn_T1A2/docs/website_screenshot/blog /phone.png

- Contact desktop

	/gysohn_T1A2/docs/website_screenshot/contacnt/desktop.png

- Contact tablet

	/gysohn_T1A2/docs/website_screenshot/contacnt/tablet.png

- Contact phone

	/gysohn_T1A2/docs/website_screenshot/contacnt/phone.png

# Target audience

The target audience for this website are the following:
- coder academy
- potential employers
- fellow developers
- friends
- family
- anyone that is interested in my journey 

# Tech stack (e.g. html, css, deployment platform, et
	- VS code - for the code writing
	- git hub - staging
	- netlify for make it live
	- scss for style
	- html6 for web content 
	- Loom to create my video 
	- Youtube to publish my video


## Version 2 26/12/23
**Home page**
I have decied to make a new home page during my holiday. 

I saw this layout and thought it would be fun to make. 

https://codepen.io/ettrics/full/ZYqKGb/

The new home page will be called home2.html

T=

**Blog page**
I actually want to start writting a blog about my education and what I am learning. So planning to find a plug that I can use to post a blog on to the webiste. I might do this during the holiday as well. But not sure If I have time 


# References
W3C Markup validation service (no date)
	https://validator.w3.org/nu/?doc=https%3A%2F%2Fgysohn.com%2F (Accessed: 18 November 2023)
Fontawseome (no date)
	https://fontawesome.com/icons (Accessed: 14 November 2023)


