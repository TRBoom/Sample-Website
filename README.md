# Assignment: Bootstrap Layout & Basics
In this assignment, you will build a basic site with grid layout in *Twitter Bootstrap*.

## Prerequisites
* Understand the basics of responsive grid layout in *Twitter Bootstrap*.
* Be able to utilize the Bootstrap utility classes.

## Objectives
* Implement a responsive layout in Bootstrap given site sample.
* Utilize Bootstrap utility classes.
* Practice HTML/CSS skills.

## Instructions
### Project Repository
A repository will be created for you automaitcally after accepting the assignment (link in Blackboard). When accepting the assignment, be sure to select your name from the list of students.

After you have accepted your assignment, navigate to the repository URL that was created and clone the repository to your local computer.

### Page Specifications
The page to be developed in this assignment is a landing page for a barer shop named "Essential Cuts". The site is divided into the following sections.
* Banner - Holds welcome message and large background image as well as a "make appointment" button.
* Barbers - Contains a profile of 3 barbers at "Essential Cuts".
* Services - Section describes a couple of services that the shop offers.
* Footer - Contains copyright and contact information.

Starter HTML has been provided as well as all the images used in the project (in the *img* folder).

### Responsive Design
The finished site should be responsive. On small and extra small screens, the layout is stacked as shown below. Notice that most of the content is centered at this screen size.

<figure>
    <img src="docs/img/finished-xsmall-small.png">
    <caption>Extra small and small screens</caption>
</figure>
---

On medium size or larger screens, the layout changes and should be similar to the image below.

<figure>
    <img src="docs/img/finished-medium-larger.png">
    <caption>Medium screens and larger</caption>
</figure>
A couple of things to note in each section.

* Banner - Has a column of width 8 and text is left aligned (we do not use the remaining 4 columns).
* Barbers - 3 equal width columns.
* Services - 2 rows with 2 equal width columns each.
* Footer - 1 row with 3 equal columns.

Also note the starter HTML in *index.html*. Look at the HTML for each of the main sections we discussed. You will notice that each section includes a container within rather than one contianer on the outside of the entire page.

``` html
<section id="barbers">
    <div class="container">
        Your content here ...
    </div>
</section>

<section id="services">
    <div class="container">
    </div>
</section>
```

This placement of the containers in each section allows for the background (color or image) to span the full width of the screen while maintaining consistent margins on the left and right. It is wihin these containers that you will layout each section with the grid system.

### Tips & Tricks
You will need to use the included CSS file to implement custom styles that cannot be implemented with Bootrap classes. What is included in here will vary according to implementation, but at the least you should have styles for the following ...

Banner - Bootstrap does not have a mechansim to include background images from HTML. You will need to implement a style here.

Section background colors - The background colors we are using in each section should be specified in the applicable CSS selector for the section.

Buttons - We did not cover the styling for buttons, but it is fairly simple. To style a button with bootstrap, do the following ...

```html
<!-- Solid button -->
<button class="btn btn-primary">

<!-- Outlined button -->
<button class="btn btn-outline-primary">
```

The standard color suffixes may be used when specifying color (i.e. primary, secondary, warning, etc.).

Finally, when placing images in the "Barbers" section, make sure to give them a class of w-100 so that they resize appropriately when the screen does. In the services section ,give a class of w-100 and h-100 to constrain the dimensions on resize.

## Submission
Submission instructions will be given during next class.