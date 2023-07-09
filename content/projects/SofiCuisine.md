---
title: "SofiCuisine PT.1"
date: 2023-07-09T18:30:19+01:00
draft: false
hideMeta: true
---

## SofiCuisine - The ultimate cooking recipes manager ( for me, of course )

I'm thrilled to share a small but exciting programming project that I'm embarking on.

This project is an exciting opportunity for me to apply my programming knowledge and develop a solution for me and my lovely girlfriend ( Sofi ) and our lack of organization in the kitchen and weekly groceries.

### État de l'art

The main ideia for the base project is to create a recipes manager with 5 simple features:

- Add, Remove and Update Recipes with bulk adding from different sources, as manual, scrapping books, websites and consume API's.
- Have dinamic properties to recipes, like, we can create different entities to classify our recipes.
- Schedule weekly our monthly meals. ( maybe integration with google calendar )
- Make a grocery list from weekly/monthly schedule. ( in several formats, maybe integrate with a notes application )
- Basic role and permissions system so we can controll all the aplication.

### Inital Stack ( can change )

 - Backend:
    - Laravel 10*
 - Frontend:
    - Nuxt 3*
 - Database:
    - MySQL 8*
 - Mobile Application:
    - 🙈 🙈 🙈 🙈

### Let's begin

#### Entity–relationship Model V1

As i said, i want to make the system the most dinamic possible for the final user ( Sofi and me ). For that i added a entities recipes table with a pivot table to work as a dynamic table. 

<a href="/images/ERD_base_v1_recipes_entities.jpg" target="_blank">
  <img src="/images/ERD_base_v1_recipes_entities.jpg" alt="Recipes Entities Diagram">
</a>

I used the same ideia for the ingredients table. 

<a href="/images/ERD_base_v1_ingredients.jpg" target="_blank">
  <img src="/images/ERD_base_v1_ingredients.jpg" alt="Ingredient Entities Diagram">
</a>

The schedule *module* will be very simple, and probably i will have to change it if in future if i want to integrate with Google Calendar or something like that.

<a href="/images/ERD_base_v1_schedule.jpg" target="_blank">
  <img src="/images/ERD_base_v1_schedule.jpg" alt="Schedule Diagram">
</a>


For permissions i will use the **spatie/laravel-permission***  because i don't want to reinvent the wheel and isn't my main focus on this project.

<a href="/images/ERD_base_v1_schedule.jpg" target="_blank">
   <img src="/images/ERD_base_v1_spatie_permissions.jpg" alt="Spatie Permissions Diagram">
</a>

You will see that i don't have a place to record multimedia, because i'm still working on that, and choosing the service that i will use to store it.

For now, that's it, i will put the flows on *paper* and start my epic (so-so) journey.


Useful links: 
<a href="https://laravel.com/" target="_blank">Laravel</a> |
<a href="https://nuxt.com/" target="_blank">Nuxt</a> |
<a href="https://www.mysql.com/" target="_blank">MySQL</a> |
<a href="https://github.com/spatie/laravel-permission" target="_blank">spatie/laravel-permission</a>
