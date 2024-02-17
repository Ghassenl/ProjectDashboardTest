# Technical test

## Introduction

Fabien just came back from a meeting with an incubator and told them we have a platform “up and running” to monitor people's activities and control the budget for their startups !

All others developers are busy and we need you to deliver the app for tomorrow.
Some bugs are left and we need you to fix those. Don't spend to much time on it.

We need you to follow these steps to understand the app and to fix the bug : 
 - Sign up to the app
 - Create at least 2 others users on people page ( not with signup ) 
 - Edit these profiles and add aditional information 
 - Create a project
 - Input some information about the project
 - Input some activities to track your work in the good project
  
Then, see what happens in the app and fix the bug you found doing that.

## Then
Time to be creative, and efficient. Do what you think would be the best for your product under a short period.

### The goal is to fix at least 3 bugs and implement 1 quick win feature than could help us sell the platform

## Setup api

- cd api
- Run `npm i`
- Run `npm run dev`

## Setup app

- cd app
- Run `npm i`
- Run `npm run dev`

## Finally

Send us the project and answer to those simple questions : 
- What bugs did you find ? How did you solve these and why ? 
- Which feature did you develop and why ? 
- Do you have any feedback about the code / architecture of the project and what was the difficulty you encountered while doing it ? 

# Les Bugs : 

Bug 1 : Dans user/list.js à la ligne 132 changer username par nom

Bug 2 : Dans user/view.js corrigez le bouton de mise à jour en remplaçant onChange par onClick


Bug 3 : Dans projects/view.js à la ligne 75 changer project.name.toString() par project.name?.toString() 

Bug 4 : Dans projects/views.js à  la ligne 26 changer       const { data: u } = await api.get(`/project/${id}`); par const { data: [u] } = await api.get(`/project/${id}`); car data c'est un array

Bug 5 : Dans projects/edit.js le meme bug que celui du Bug 4 mais sur la page edit 

Bug 6 : lors de la creation d'un nouveau projet la liste rafraichi auto maintenant

# Feature ajouté : 

j'ai ajouté une fonctionnalité qui permet de rattacher des Users à un projet pour faciliter de comprendre qui sont les personnes qui travaillent sur ce projet.

# Temps de travail : 

20 minutes : fixing the bugs

30 minutes : ajout de la nouvelle Feature.

