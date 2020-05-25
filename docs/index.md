
# Specifications of BioPrime

## A repository for keeping record of the primers in a Biobank

### First Introduction

The document describes the specifications of the repository BioPrime for computerisation of biobanks for primers. The respository is a system for organised management of informations about the primers, the existing stocks of primers in the laboratory and their location there. It will simplify the ordering and the recording of the consumption of primers. It will also provide a way better trasparency of the analyses of the companies and ease their everyday work.

Good documentation constitutes an essential part of the quality assurance system and is key to operating in compliance with GMP requirements, so with this document we provide you a description of the functions of the repository, instructions and procedures, written in an instructional form. The document contains:

* review of the repository with a use – case diagram
* detailed description of user access control
* functional requirements of individual parts of the repository (system functionality)
* user view, that represents the final appearance of the repository

### Review of the repository

#### Use - case diagram

![userTypes](./userTypes.jpeg)

### Users access

A new user is created by the Administrator, who also provides the username (or new users log in with an already existing email) and password. He also sets the user's role and their level of access.  As written before, different users will have different roles in the repository, which controls their information access. The roles are:

* Guest / General user
* Student
* Laboratory Technician
* Researcher / Lab Staff
* Administrator

#### Guest / General user

A Guest / General user will have the access to primer data (view only) and will be able to export data.

#### Student

A Student will have access to primer data (view only) and history view. They will be able to export data and modify primer volume.

#### Laboratory Technician

A Laboratory Technician will have access to primer data (view only) and history view. They will be able to import  (but not export), order new / reorder primers and modify primer volume and state (formulation).

#### Researcher / Lab Staff

A Researcher / Lab Staff will have access to primer data (view only) and history view. They will be able to import and also export data, to add or remove primers, modify primer data, volume and state (formulation) and order new / reorder primers.

#### Administrator

The Administrator will have access to primer data (view only) and history view. They will be able to import and also export data, to add or remove primers, modify primer data, volume and state (formulation) and order new primers / reorder primers. They will see the users overview and be able to add or remove users, modify  access level of users and modify their roles.

## System Functionality

We divided the system functionality into specific sections:

* Login Page
* Access to Primer Data Library
* Searching and Sorting Primer Data
* Adding New Primers
* Customizing Primer Data
* Ordering New Primers
* Analysis

## Login Page

When you access the BioPrime website, it first takes you to the login options. All repository users need to log in before viewing or costumizing data.

![login_screen](./login_screen.JPG)

New users and their assigned roles are created by the Administrator. Users are then notified by e-mail about their access grant. Personal or work e-mail can be used as the username and the password should be set by the users themselves.

If the password has been forgotten or the e-mail has been changed, the Administrator can permit the option of creating a new password, change the role of the user or delete them and add them with a new e-mail.

## Access to Primer Data Library

After logging in, the user is presented with the main page of the program.

![dashboard](./dashboard.png)

Icons on the left show:

* Dashboard, which is the main page showing primer data
* Orders, where recent and pending orders can be viewed
* History, which shows a timeline of all changes made by the users (view limited only to specific users)

![menu1](./menu1.png)

The Administrator also has access to the "Manage Users" section.

![admin](./admin.png)

Dashboard view shows general analysis data on top of the page, including the occupancy of refrigerators and the total number of primer.
Primers are presented in a list and automatically sorted by their Generated name in an ascending order. The order can be modified based on any trait (such as Sequence, Freezer, User etc.), described in detail in the following chapter.
Only the desired amount of primer data is shown, which can be by checking off boxes in the "View Columns" section in the top right corner. User can also use the option of "select all" to see all the data at the same time.

Details of each primer can be viewed by clicking the box on the left of each primer then choosing "Open Data" on the top right.

![access1](./access1.png)

This way primers can also be modified or deleted, if your assigned role allows you that option. This is described in the Costumizing primer data section.

## Searching and Sorting Primer Data

Search options include normal and advanced search options.
When using normal search, the user can search solely by the gene.
Advanced search can be done by clicking on the "Filter Table" button on the top right, search under these traits is available:

* ID of primer
* Generated name of primer
* Organism
* User
* Type of primer
* Project

Primers can be sorted based on certain traits by clicking on the "View columns" button on the top right and checking off the boxes with desired traits, then clicking the name of the trait on top of each column to sort based on ascending order and double clicking for descending order.

## Adding New Primers

New primers are added with a click on the "Add" button on the top right. The system offers you to add one or two primers at the same time. If you simply want to upload a document you can click on the "CSV" option and upload your file on to the database.

| Obligatory Data | Optional Data |
|-------|-------|
| Name of primer  | NCBI gene ID  |
| Sequence | Human genome build|
| Organism  | Length |
| Gene  | Tm (℃)  |
| Position in the reference | Optimal T of annealing (℃) |
| Formulation | GC (%)  |
| Purification method | Storing T (℃)   |
| Type of primer | Sonda Sequence (for TaqProbe)   |
| Application  | Length of amplicon  |
| 5' modification | Amount available  |
| 3' modification  | Did you check specificity in blast? |
| Location  | Designer |
|  | User |
|  | Project |
|  | Supplier |
|  | Manufacturer |
|  | Date |
|  | Comment |
|  | Analysis |

![add_primer1](./add_primer1.JPG)

![add_primer2](./add_primer2.JPG)

![add_primer3](./add_primer3.JPG)

When adding a new primer, user can choose between adding a single primer or a pair (forward and reverse). When putting in data for a pair of primers, common features are put in first, specific features for each primer are:

* Name of primer (obligatory)
* Position in the reference (obligatory)
* Length
* Tm (℃)
* Optimal T of annealing (℃)
* GC %
* Storing T (℃)
* Sequence (obligatory)
* 5' modification (obligatory)
* 3' modification (obligatory)
* Location (obligatory)
* Comment

When adding a TaqProbe, extra options for putting in data open up:

* Assay ID
* Size
* Sonda Sequence
* Quencher
* Dye

"Sequence" is also not among obligatory data for TaqProbes.

A document can also be added to the primer data, for example a sheet of information provided by the manufacturer.

## Customizing Primer Data

After opening the primer details, you can edit the data by clicking on the editor icon.

![access2](./access2.png)

This allows you to add a comment, manage the primer volume or formulation or correct any possible mistakes that were made when adding a new primer into the repository. The amount of editing that is allowed is based on the users' assigned role.

## Ordering New Primers

If less than 10 µL of primer are available a new order should be made immediately.

After completing an order, the date of order appears in the data of a specific primer.
Existing orders can be viewed in the "Orders" page, accessible on the top left of the site. Under it is a "Wanted Oligonucleotide Primers" section, where the user can view all the primers pending to be ordered and when enough material from the same supplier is under "wanted", everything can be ordered in a batch.

![orders](./orders.png)

Before adding a new order, this page should be checked so the orders don't overlap. If the primer has already been order this is also shown under "primer details" (described in the "Access to primer data library" section).
If the order is the first one from the batch, it can be added as a pending order under the "Wanted Oligonucleotide Primers", this allows other users to add their wishes and all the primers can be ordered in a batch. This is done by selecting a primer and then clicking "Move to ordered primers" after ordering.

![orders2](./orders2.png)

### Analysis

![database-diagram](./database-diagram.png)

-------------
