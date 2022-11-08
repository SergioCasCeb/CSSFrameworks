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

* The default development build of Tailwind CSS is 2413.4kB uncompressed, and 190.2kB minified
* Tailwind automatically removes all unused CSS, ultimately giving a much smaller CSS file for production
* They cound with their own [playground site](https://play.tailwindcss.com/) to test their utilities
* Used by more than 2.8 m people and with 255 contributors ( [Github](https://github.com/tailwindlabs/tailwindcss) )
* MIT license for their simple utility classes
* Tailwind UI Personal Package: one payment of 249 Euros (500+ components, site templates, and lifetime access)
* Tailwind UI Teams Package: one payment of 749 Euros (Everything in the personal package but with access for up to 25 people)
* Constant bug fixes and maintenance (The latest version as of 08.11.2022 is v3.2.2 released on 05.11.2022)


| Advantages  | Disadvantages |
|     ---     |    ----     |
| Minimal CSS | In order to create a more unique feeling it could be necessary to overwrite and create many personalized values |
| Flexible and easily customizable | With all the default values the build can take up an average between a few miliseconds to 5 seconds | 
| Consistent layout and overall feeling | Animations, transitions and pseudo-classes (hover, focus, etc.) might require personalized code for better functionality |
| Wide variety of default utilities | A higher learning curve for people who only have a basic knowledge of CSS or no knowledge at all, in comparison to other frameworks |
| (Some) Free and easy to implement pure CSS components ||

## [Bootstrap](https://getbootstrap.com/)
