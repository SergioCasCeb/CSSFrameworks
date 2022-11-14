# Possible CSS Frameworks/UI Libraries for Playground

After analyzing the most popular CSS frameworks/UI LIbraries of the last few years such as: Tailwind CSS, Bootstrap, Foundation, UI Kit, Materialize, Bulma, Skeleton, Pure CSS, Semantic UI, etc. I personally believe that UI libraries would not be the best approach to redesigning the Playground site due to their constraints regarding customization and scalability. 

While a UI library provides you with "professional" looking components that cater to specific behaviors and allows for easy prototyping, such components will always behave how they were created and will only allow for simple theme changes (font sizes, colors, border radius, etc). Therefore if a component can no longer fulfill the required tasks or specs of the projects, the most common ways to solve this are to override the components completely or find ways to work around them which is often time-consuming and might still not allow for the full customization that was expected.

Another important fact to have in mind is that all the components rely heavily on their respective intended frameworks and versions, which could force the use of specific older versions to assure functionality, compromising the looks and feel of the components themselves, which in my opinion beats the purpose of the redesigning process that is trying to be achieved with this project.

Contrary to UI libraries, CSS frameworks, which as the name implies, are mostly based on isolated reusable styles and classes making them easier to modify and override. Even though also being restrictive to certain extemp it can be argued that such restrictions help to create a more consistent layout and feel overall.

In a nutshell it can be said, that UI libraries are helpful for quick prototyping, accepting that certain behaviors will remain constant and the main focus is mostly to find a way to interact with data compromising the looks and feel of the site/app. And CSS frameworks are useful when specific behaviors are needed or wanted, or when there's a need to have more control over the code in order to achieve a specific feel or look.

With this in mind, I picked the 4 Frameworks that, in my opinion, could be a useful addition to the project, considering characteristics like package size, price/license, popularity, responsiveness, utilities and components as well as flexibility/customizability.

## [Tailwind CSS](https://tailwindcss.com/)

A utility-first CSS framework that allows for lots of flexibility as well as customization. Tailwind provides a wide arrange of default classes ranging from colors, spacing, and typography to responsiveness, grid/flex layouts, hover and focus states, etc. which helps keep an overall consistent design system. Nonetheless, if such classes are not enough for the project, or it's necessary to add some custom values, tailwind allows for an easy way to add custom utilities as well as arbitrary values.
Tailwind also counts with pure css custom components and templates, and even though most of them are blocked behind a pay wall, they do offer a few free examples that can be easily implemented in any project.

Even though the development build of Tailwind CSS is 2413.4kB uncompressed, and 190.2kB minified, which sounds like a lot, it is only due to the thousands of utility classes the tailwind generates in order to make the experience as productive as possible. Nonetheless, such utilities can always be overwritten to only use the values that the project at hand requires.

When it comes to production though, because tailwind is incredibly performance focused and aims to produce the smallest CSS file possible, it usually leads to CSS files that are less than 10kB, as claimed by [Tailwind CSS](https://tailwindcss.com/docs/optimizing-for-production).


**Characteristics:**

* Size: The default development build of Tailwind CSS is 2413.4kB uncompressed, and 190.2kB minified (Final CSS file >10kB)
* Installation: Simple installation through Tailwinds CLI, CDN (Not recommended for production), as a PostCSS plugin, and it also includes framework specific guides
* License: MIT license for all their utilities and certain components and templates
* Paid Packages: 
  * Tailwind UI Personal Package: one payment of 249 Euros (500+ components, site templates, and lifetime access)
  * Tailwind UI Teams Package: one payment of 749 Euros (Everything in the personal package but with access for up to 25 people)
* Popularity: Used by more than 2.8 m people and with 255 contributors ( [Github](https://github.com/tailwindlabs/tailwindcss) )
* Maintenance: Constant bug fixes and maintenance (The latest version as of 08.11.2022 is v3.2.2 released on 05.11.2022)
* Tailwind automatically removes all unused CSS, ultimately giving a much smaller CSS file for production
* They count with their own [playground site](https://play.tailwindcss.com/) to test their utilities


| Advantages  | Disadvantages |
|     ---     |    ----     |
| Minimal and modular CSS | In order to create a more unique feeling it could be necessary to overwrite and create many personalized values |
| Flexible and easily customizable | With all the default values the build can take up an average between a few miliseconds to 5 seconds | 
| Consistent layout and overall feeling | Animations, transitions and pseudo-classes (hover, focus, etc.) might require personalized code for better functionality |
| Wide variety of default utilities | A higher learning curve for people who only have a basic knowledge of CSS or no knowledge at all, in comparison to other frameworks |
| (Some) Free and easy to implement pure CSS components ||

## [Bootstrap 5](https://getbootstrap.com/)

Bootstrap is a leading free, open-source front-end development framework for the creation of responsive websites and web applications. Although it is a front-end framework it is often referred to as a CSS Framework. This framework comes with a responsive grid system based on flexbox, global CSS variables, extensive pre-built components and utilities, and JavaScript plugins to speed up the development process. It is also possible to include either just the CSS or the JavaScript compiled files.

Since the release of Bootstrap version 5, it does not longer require the use of jQuery and it utilizes SASS as its CSS preprocessor to handle all its global values, utilities, and components which can also be overwritten and customized.

In comparison to Tailwind CSS which is a pure CSS framework, Bootstrap has a few components that rely on specific JS plugins in order to handle certain specific behaviors. Nonetheles most of the components and utilities can be used and accessed just by using their CSS files.
It is also worth noting that contrary to Tailwind which makes sure only the necessary CSS is being used, Bootstrap includes every single value, utility, and component unless it is explicitly removed or overwritten.

**Characteristics:**

* Size: The default bundle size of Bootstrap CSS (no JS) ~20kB compressed and ~116kB uncompressed
* Installation: It can easily be included via CDN, installed via the package manager, or by downloading the source code
* License: Completely free to use (MIT license)
* [Premium templates](https://themes.getbootstrap.com/) for sites and dashboard (around $49)
* Popularity: 
  * Bootstrap is the eighth most starred project on GitHub, with over 158,000 stars
  * Over [21 million websites use Bootstrap](https://trends.builtwith.com/docinfo/Twitter-Bootstrap)
* Maintenance: Constant bug fixes and maintenance (The latest version as of 08.11.2022 is v5.2.2 released on 03.10.2022)
* Completely responsive and mobile first

| Advantages  | Disadvantages |
|     ---     |    ----     |
| Wide options of components | Some components rely on JS |
| Fully responsive (mobile first) | Components and utilities can be complicated to work around | 
| Defalt JS pluging to handle behaviors | Knowledge in SASS is necessary to personalize components |
| Easy to learn and start implementing | If not removed explicitely all default utilities and components are added to the CSS |
|  | Even though some components handle hover and focus animations, there is no given way to modify this, so to have personalized animations and transitions have to be added normally in the CSS |

## [Bulma](https://bulma.io/)

Bulma is a free, open-source CSS framework built primarily with Sass and a Flexbox system. It offers modular columns and it provides some default utilities for rapid UI development.

Bulma is completely responsive, and like Tailwind CSS is also modular, allowing the use of only the components and utilities that the project might require. Nonetheless, unlike Bootstrap, Bulma is a CSS pure framework, meaning that the behavior and event handling that the project might require has to be added personally.

Finally, Bulma has a really simple, readable, and easy-to-use naming system for its utilities and components, which makes it easier for everyone to understand what each class is doing.

* Size:The size of bulma v0.9.4 is 201.9 kB (minified), and 26.9 kB when compressed
* Installation: Can be installed through NPM, Yarn and Bower or directly downloaded from their website and github
* License: Completely free to use (MIT license)
* Popularity:More than 200k users
* Maintenance: Constant bug fixes and maintenance (The latest version as of 08.11.2022 is v0.9.4 released on 08.05.2022)
* Completely responsive with a mobile-first approach


| Advantages  | Disadvantages |
|     ---     |    ----     |
| Fully responsive (mobile first)  | No behavior and event handling |
| Easy to learn and understand  | It requires the use of Sass to customize the utilities | 
| Modular  | The default values only cover a really basic amount of values |
| Flexible and easily customizable  | No hover, transitions or animation utilities |

## [Skeleton](http://getskeleton.com/)

As implied by its name, Skeleton more than a CSS or UI Framework, and as stated on their official [Github](https://github.com/dhg/Skeleton), " Skeleton is a simple, responsive boilerplate to kickstart any responsive project".
Skeleton is perfect for smaller projects (minified size of 176 B) that don't require much setup or when all the utilities from bigger frameworks seem too much for the project at hand. Skeleton only styles a few standard HTML elements (typography, buttons, forms, lists, code, tables), it has a simple 12-column grid system, 4 utilities to handle the width and float and it can also handle media queries.
Since it is just a boilerplate it doesn't require any maintenance, hence why the last release was in 2014.

**Characteristics:**

* Size: Minified size of 176 B
* Popularity: 18.7k stars on Github
* License: Completely free to use (MIT license)
* Maintenance: Last updated on 2014

| Advantages  | Disadvantages |
|     ---     |    ----     |
| Incredibly light size  | Grid system that still relies on float |
| Easy to use | minimal utilities | 
| Supported by all modern browser versions and most older versions | Non-scalable |
| Responsive | In more complex projects that require specific customization, most if not all components and utilities will just end up being obsolete |
||Last time it was modified/updated was on 2014|
