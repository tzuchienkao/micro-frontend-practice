---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://www.thespian.hr/png/micro-frontends-without-javascript-components.png
# apply any windi css classes to the current slide
class: 'text-center bg-transparent'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## What Micro Frontend
  Sharing for developers after Frontend Conferences.

  #LV
# persist drawings in exports and build
drawings:
  persist: false

---
<style>
.slidev-layout {
  background-color: #fdcf95;
  color: white;
}
ul, ol, li {
  list-style: none;
}
h1 {
  color: #146b8c;
}
</style>
---

# What are Micro Frontends?

<h4>The End Of 2016</h4>
<p>First came up in ThoughtWorks Technology Radar.</p>


<h4>Concepts</h4>
<p>The idea behind Micro Frontends is to think about a website or web app as a composition of features which are owned by independent teams.<br>Each team has a distinct area of business or mission it cares about and specialises in.<br>A team is cross functional and develops its features end-to-end, from database to user interface.</p>

---

<h4>Core Ideas behind Micro Frontends</h4>

- **Be Technology Agnostic**
  + Each team should be able to choose and upgrade their stack without having to coordinate with other teams.<br>Custom Elements are a great way to hide implementation details while providing a neutral interface to others.

- **Isolate Team Code**
  + Don’t share a runtime, even if all teams use the same framework.<br>Build independent apps that are self contained.<br>Don't rely on shared state or global variables.

- **Establish Team Prefixes**
  + Agree on naming conventions where isolation is not possible yet.<br>Namespace CSS, Events, Local Storage and Cookies to avoid collisions and clarify ownership.

- **Favor Native Browser Features over Custom APIs**
  + Use Browser Events for communication instead of building a global PubSub system.<br>If you really have to build a cross team API, try keeping it as simple as possible.

- **Build a Resilient Site**
  + Your feature should be useful, even if JavaScript failed or hasn't executed yet.<br>Use Universal Rendering and Progressive Enhancement to improve perceived performance.

Read more about [Micro Frontends](https://micro-frontends.org/)
