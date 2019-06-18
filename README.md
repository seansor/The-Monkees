# The Monkees

User-Centric Frontend Development Milestone Project - Code Institute 

This is a website for the band The Monkees. The website allows fans and potential fans to see and hear clips from the band's back catalog, 
and any new material as it becomes available, as well as keep up to date with the latest news and upcoming tour dates. The website also
includes some background on the band and band members, a gallery to view photos and pictures and a contact page.



## UX

My goal was to provide fans and potential fans with a website where they could easily listen to the band's music, find out about upcoming
live shows and keep up to date the latest band news. In keeping with the band's image of fun and frivolity, I wanted to include fun images 
and colours throughout the website. The red-orange (primary) and yellow (secondary) colours used in the website are also in keeping with
the theme and colour scheme used by the band on logos and album art, which are familiar to fans. As the band were the result of an old tv
show I wanted the website to contain lots of images and pictures that would evoke good memories for old fans and give a sense of the band
to potential fans.

As many users will only visit the homepage of a website I wanted to ensure the most important information was readily available on this page.
I identified the most important items as:

    - links to the main media/streaming services (apple music, spotify, etc.)
    - Latest Release (via video)
    - Upcoming live shows
    - Latest news
    
On 'The Band' page I wanted users to see a picture of the band with a brief overview, followed by a section on each band member inlcuding
their picture, role in the band, and a short biography.

On the 'Music' page I wanted users to first see the latest album release with a link to listen to the album on a streaming service.
However I also wanted users to be able to listen to music directly in the music page so I provided audio for four of the "Top Tracks"
and a "More tacks" section. Finally on this page, I wanted users to also be able to enjoy some of the music videos.

As mentioned above, The Monkees band have been around for a long time and are the result of a tv show by the same name. I wanted fans to
be able to enjoy looking at old photos of the band and Monkess images such as album art. For this reason I included a gallery page.

On the 'Live' page the users will see more live concert dates, their location and venue. They will have a link for each show which will take
them to the official ticket sellers webpage.

Finally the 'Contact' page provides users with a method of getting in conact with the band. Users are provided with a selection of
social media links for this purpose. Promoters or event organisers enquiring about availability are provided with a short form which can
be quickly filled out. The form allows users to select the event type, estimated number of people and provide their contact details.

The footer provides the user with the ability to sign up to recieve email updates about the band by entering their email address.
It also provides links to all of the band's social media accounts.


## Technologies
1. HTML
2. CSS
3. Bootstrap (4.3.1)



## Features

The website uses Font-awesome (4.7.0) to add icons and enhance the visual appearance of the website.

An animation was used to transition in the navbar from the top of the page.

The red buttons on the pages such as "Read More", "Tickets", etc. provide the users with links to external websites to carry out the
stated function on the button (e.g. read more [news] or [purchase concert] tickets). The white and grey buttons provide the users 
with links to other pages within the website. At all times the Monkees Icon in the top left corner can be used to navigate back to the homepage.

The latest album release on the Music page has been set up so that an overlay appears on hover asking the user if they want to listen
to the album on Apple Music.

The gallery page uses Fancyapps Fancybox (3.5.7) so that the thumbnails provided enlarge to their actial size and can be easily
navigated through with simple backwards/forwards arrows.

The video iframes allow the users to watch videos on the website without slowing the website down unduly by directly adding video content.

The music/audio controls on the Music page allow users to listen to the "Top Tracks". The Apple Music iframe allows the user to listen to more
tracks without having to directly include dozens of mp3 files on the site.

The contact page allow event organisers to request availability quickly and easliy by filling out a short form.

The footer provides the user with the ability to sign up to recieve email updates about the band by entering their email address.


### Features Left to Implement

At a future date I would like to add a link to the bands online store.

I would also like to incorporate a Spotify player (as well as the Apple Muisc player provided) and give the user the ability to choose their
preferred player.


## Testing

*All testing was done manually*

#### Universal/General (Common to multiple pages)

All buttons and links are functioning and point to the correct destination. All links to other webpages will open in a new tab using 'target="_blank"
Navigation menu and toggler work as expected.
All images are displayed correctly and do not unintentionally obscure any other content.
All music files play and stop with when relevant controls are selected. Download music link on audio players work.
All iframes show video (or other content) content correctly.

#### Homepage

The links on the homepage to the main media/streaming services all work and point to the correct destination. The Latest Release video plays.
The "Upcoming Live Shows" section clearly identifies the upcoming shows and the links to purchase tickets are functioning properly. The Latest
News section displays the article headline and the "Read More" links are functioing and point to the correct destination.

#### The Band 

'The Band' page displays pictures correctly. Text and pictures positioning are correct.

#### Music 
An opaque overlay asking if the user wants to listen on Apple Music appears on hover over "The latest album release". The associated link 
functions correctly.
The audio controls for the "Top Tracks" function as expected. 
The Apple Music iframe in "More tacks" functions as expected. 
The music videos on this page all function properly.

#### Gallery 

All gallery thumbnails are displayed correctly. The fancybox tool works to enlarge the photos to their actual size and provides a
navigation window for the photos.

#### Live

The Live concert dates, their location and venue are all displayed correctly. The link to buy tickets functions and directs to the correct
destination.

#### Contact

The social media links all work and direct to the correct destinations. for this purpose. The form works as expected. If you try to submit
the form with an invalid email address, there will be an error noting the invalid email address. Furthermore, the 'required' attribute
is added to the 'name, 'company', 'phone', 'email', and "T&Cs"  so if those fields are not filled in, the form will not submit.
If all field are valid, the page will reload.

#### Footer
The "Get Updates" field works as expected. If you try to submit the form with an invalid email address, there will be an error noting the
invalid email address.
The links to all of the band's social media accounts function and point to the correct destination.

### Responsiveness and cross platform operation

The website has been tested for a wide range of screen sizes and all items display well across these screen sizes. Some items are hidden
on dictated screen sizes (dictated via media queries). The images and content layout change based on screen size. The video iframes 
are responsive and take up 66% of the screen width on large screen and close to 100% on mobile devices while maintaining their aspect ratio.

The navbar collpases to a toggle icon on mobile devices. The dropdown background displays darker to make the nav-items stand out from the
background image.

The site was tested across multiple browsers (Chrome, Safari, Internet Explorer, FireFox) and on multiple mobile devices
(iPhone 5, 6/7/8, 6/7/8plus, X; Chrome and Safari, iPad, iPadPro Samsung Galaxy, OnePlus) to ensure compatibility and responsiveness. 
During the testing I notices that on the IPad Pro the audio controls were pushed too close together and were causing a margin on the RHS of 
the Music Page. To fix this, I edited the media query so that the Top Tracks were displayed 2-across rather than 4 across on devices below a 1200px
width (as was the case previously for devices below 1025px.)

I also noticed during testing that when the website was deployed some of the images were not displayed even though they had been showing when run
from C9. To fix this I had to explicitly point to the current directory by using './assets/...' rather than just '/assets/...'.


## Deployment
This site is hosted using GitHub pages, deployed directly from the master branch. The deployed site will update automatically upon new commits
to the master branch. In order for the site to deploy correctly on GitHub pages, the landing page must be named `index.html`.

To run locally, you can clone this repository directly into the editor of your choice by
pasting 'git clone https://github.com/seansor/The-Monkees.git' into your terminal.
To cut ties with this GitHub repository, type `git remote rm origin` into the terminal.


## Credits

### Content

The content in 'The Band' page is taken from [Wikipedia](https://en.wikipedia.org/wiki/The_Monkees).

### Media

Images were used from the project assets folder provided. Also images were taken from the following sources:
    -[Wikipedia](https://en.wikipedia.org/wiki/The_Monkees)
    - www.mentalfloss.com
    - https://www.billboard.com
    - grunge.com
    - metv.com
    - newsmax.com
    - pinterest.com
    - bbc.co.uk
    - nytimes.com
    - wbur.org
    
    *The images are used for an educational project and are not intended for commercial reuse*
    
Audio (mp3) files from the assets folder provided were used.

### Acknowledgements

[Bootstrap](https://getbootstrap.com/ (4.3.1) was used for the navigation bar, for the table in the live dates section and for the form
in the contact section, all of which were edited to meet the websites needs. Bootstrap was also used to assist in page layout.

[Fontawesome](https://fontawesome.com/v4.7.0/icons/) was used for icons.

[Fancybox](http://fancyapps.com/fancybox/3) was used for the gallery's image navigation feature.
