
# Specifications of BioPrime

## A repository for keeping record of the primers in a Biobank

### Introduction

The document describes the specifications of the repository BioPrime for computerisation of biobanks for primers. The respository is a system for organised management of informations about the primers, the existing stocks of primers in the laboratory and their location there. It will simplify the ordering and the recording of the consumption of primers. It will also provide a way better trasparency of the analyses of the companies and ease their everyday work.

Good documentation constitutes an essential part of the quality assurance system and is key to operating in compliance with GMP requirements, so with this document we provide you a description of the functions of the repository, instructions and procedures, written in an instructional form. The document contains:

* review of the repository with a use – case diagram
* it describes the user access control
* functional requirements of individual parts of the repository
* zaslonske maske (prevod v angleščini) , that represent the final appearance of the repository

### Review of the repository

#### Use - case diagram

![userTypes](./userTypes.jpeg)

### Users access

A new user is created by the Administrator, who also provides the username (or we use an already existing email) and the password. He also sets the user's role and his level of access.  As written before, different users will have different roles in the repository, which controls their information access. The roles are:

* Guest / General User
* Gondola
* Student user
* Laboratory Technician
* Researcher / Lab Staff
* Administrator

#### Guest / General User

A Guest / General user will have the access to primer data (view only) and will be able to export data.

#### Student

A Student will have the access to primer data (view only) and history view. He will be able to export data and modify primer volume.

#### Gondola2

<video controls="true" autoplay allowfullscreen="true">
<source src="gondola.webm" type="video/webm">
</video>

#### Laboratory Technician

A Laboratory Technician will have the access to primer data (view only) and history view. He will be able to import data, but not export and can also order primers. He can modify primer volume and  primer state (formulation).

#### Researcher / Lab Staff

A Researcher / Lab Staff will have the access to primer data (view only) and history view. He will be able to import and also export data, to add or remove primers, modify primer data, volume and state (formulation) and order primers.

#### Administrator

An Administrator will have the access to primer data (view only) and history view. He will be able to import and also export data, to add or remove primers, modify primer data, volume and state (formulation) and order primers. He will have the users overview and will be able to add or remove users, to modify users access level and to modify users roles.

| Urban | Urban |
|-------|-------|
| test  | test  |

-------------

<iframe width="560" height="315" src="https://www.youtube.com/embed/uzvcztUmMwA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/7I0dlovDgZM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
