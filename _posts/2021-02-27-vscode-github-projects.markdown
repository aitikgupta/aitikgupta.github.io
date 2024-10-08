---
title: VSCode GitHub Projects
layout: post
date: 2021-02-27 15:10
tag:
- TypeScript
- GraphQL
- Svelte
- Extension
image: https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/001/412/509/datas/original.png
headerImage: true
projects: true
description: Bringing GitHub Projects into VSCode - using GraphQL and Svelte
category: project
author: aitikgupta
about: true
code: https://github.com/MLH-Fellowship/vscode-github-projects
externalLink: false
---

#### This project was completed as a part of [Sprint 0 Hackathon](https://fellowship-explorer-0-batch-2.devpost.com/) conducted during the [MLH-Fellowship](http://fellowship.mlh.io/) (Spring 2021).
## Insipiration
There are several utilities from GitHub that makes collaboration easy, GitHub Projects is one of them. 

Currently, there is no UI-based extension that integrates GitHub Projects in VSCode. Hence, our team (Me, [Dean Gladish](https://github.com/gladishd), [Samuel Yuan](https://github.com/yuansamuel) and [Shrill Shrestha](https://github.com/shrillshrestha)) decided to make one.

#### A quick spoiler: we [won](https://devpost.com/software/vscode-github-projects)!
## Video Demonstration (YouTube)
<iframe width="100%" height="597" src="https://www.youtube.com/embed/MycrfrHHz18" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
## What are GitHub Projects?
GitHub Projects are divided into 3 scopes:
- User Scope
- Repository Scope
- Organisation Scope

One can create Kanban boards with any of these scopes to track the progress of a project. A typical card maintained on a project board can contain anything from a simple note to linked Issues and Pull Requests.
## What does the extension do?
The [extension](https://marketplace.visualstudio.com/items?itemName=Pod212.vscode-github-projects) we built communicates with GitHub's backend using GraphQL API - Queries and Mutations, to render a WebView built by Svelte on VSCode with it's native UI.
<p align="center">
 <img alt="Extension Screenshot" src="https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/001/412/508/datas/gallery.jpg"/>
</p>
<figcaption>Sample Screenshot</figcaption>
The result is an integration of realtime communication between VSCode native UI and GitHub Projects. It allows a user to:
1. View the Projects (with filtered scopes)
2. View the Project Boards
3. Add a Project Card
4. Delete a Project Card
5. Archive a Project Card
6. Move a Project Card to a different Column
7. Edit a Project Card (Only if it is a Note)
8. Convert a Project Card ** into an Issue**
9. Visit the web version of the linked Issues/Pull Requests

<p align="center">
 <img alt="Extension Screenshot" src="https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/001/412/509/datas/original.png"/>
</p>
<figcaption>Editing a Project Card</figcaption>
## How is it built?
- WebViews built with **Svelte**
- Queries/Mutations with GitHub using **GraphQL** (**Apollo client**)
- **Session-based** GitHub OAuth
- Communication with native VSCode APIs with **TypeScript**

<p align="center">
	<img alt="Extension Architecture" src="https://user-images.githubusercontent.com/43996118/108566810-06d0c580-732d-11eb-9d06-44023673c0db.png"/>
</p>
<figcaption>Software Architecture</figcaption>

<p align="center">
	<img alt="GraphQL Schema" src="https://user-images.githubusercontent.com/43996118/108566899-2c5dcf00-732d-11eb-8782-7862b3e3a32b.png"/>
</p>
<figcaption>GraphQL Schema</figcaption>
## Project Links
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#ccc;border-spacing:0;margin:0px auto;}
.tg td{background-color:#fff;border-color:#ccc;border-style:solid;border-width:1px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#f0f0f0;border-color:#ccc;border-style:solid;border-width:1px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-xwyw{border-color:#000000;text-align:center;vertical-align:middle}
.tg .tg-0a7q{border-color:#000000;text-align:left;vertical-align:middle}
@media screen and (max-width: 767px) {.tg {width: auto !important;}.tg col {width: auto !important;}.tg-wrap {overflow-x: auto;-webkit-overflow-scrolling: touch;margin: auto 0px;}}</style>
<div class="tg-wrap"><table class="tg">
<thead>
  <tr>
    <th class="tg-xwyw">Description</th>
    <th class="tg-xwyw">Type</th>
    <th class="tg-xwyw">Link</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-xwyw">Demo</td>
    <td class="tg-xwyw">YouTube</td>
    <td class="tg-0a7q"><a href="https://youtu.be/MycrfrHHz18" target="_blank" rel="noopener noreferrer">youtu.be/MycrfrHHz18/</a></td>
  </tr>
  <tr>
    <td class="tg-xwyw">Extension</td>
    <td class="tg-xwyw">Visual Studio Marketplace</td>
    <td class="tg-0a7q"><a href="https://marketplace.visualstudio.com/items?itemName=Pod212.vscode-github-projects" target="_blank" rel="noopener noreferrer">Pod212.vscode-github-projects/</a></td>
  </tr>
  <tr>
    <td class="tg-xwyw">Submission</td>
    <td class="tg-xwyw">Devpost</td>
    <td class="tg-0a7q"><a href="https://devpost.com/software/vscode-github-projects" target="_blank" rel="noopener noreferrer">devpost.com/software/vscode-github-projects/</a></td>
  </tr>
  <tr>
    <td class="tg-xwyw">Source Code</td>
    <td class="tg-xwyw">GitHub</td>
    <td class="tg-0a7q"><a href="https://github.com/MLH-Fellowship/vscode-github-projects" target="_blank" rel="noopener noreferrer">MLH-Fellowship/vscode-github-projects/</a></td>
  </tr>
</tbody>
</table></div>
	
## Roadmap/Code/Documentation
The repository is open sourced at MLH-Fellowship's [GitHub](https://github.com/MLH-Fellowship/vscode-github-projects).
