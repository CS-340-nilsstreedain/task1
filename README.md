# DB Intro Activities
These activities are intended to give you practice building a database using SQL data definition language (DDL) and writing some simple data manipulation queries (optional).  These will also reinforce the concept of good design. There are multiple activities for this module, please complete them all.

## Video Overview
https://kaltura.oregonstate.edu/browseandembed/index/media/entryid/1_pu4d72nf

## Getting Credit for the Assignment
You will submit a file to Gradescope for testing that will be evaluated.

### [‼️] When you see this symbol, pay extra attention to what you are being asked to do in the step. In some cases deviations from the instructions can cause Gradescope to report that you did not pass. Attention to detail is required. Pay attention to the instructions and follow them closely.

## What To Turn In
You will create a file called `activity-m2.sql` and submit it to Gradescope for grading. You may resubmit as many times as necessary before the due date.

## Important Notes
Here are a few important notes to follow to ensure success on your first Gradescope submission:

### Naming Conventions
- Within an organization, consistency in the documentation of different systems promotes understanding and increases efficiency
- Including spaces in data names can create problems when writing SQL commands – so don’t do it
- Capitalizing new words increases the readability of the data names (or you may use dashes)
- Choose meaningful names so that readers will quickly get a good idea of what is stored
- Be consistent. If one table is plural e.g., vendors, all should be plural i.e., NOT invoice. Developers and users can more quickly and accurately identify items without having to verify such details

### Datatypes
MySQL has a handful of datatypes it can contain. Some are a bit more specialized than other. To see a comprehensive list of datatypes take a look at [this](https://dev.mysql.com/doc/refman/8.0/en/data-types.html). Otherwise, here are the more common ones we will be using:

Datatype | Description
---|---
VARCHAR(50) | This is a standard size text field that holds a string.
LONGTEXT | This is an enormous (~4GB max) field capable of holding a string. Use of this should be limited however, since sorting and searching operations that encounter this datatype may not return the desired results.
INT | An integer (a whole counting number, like 1, 2, 3…) and is often the choice for primary keys.
DECIMAL(X,Y) | A decimal with specified precision denoted by X and numbers after the decimal place denoted by Y. For this exercise, we will use it for money, but deeper in the exploration we discuss why this isn't the optimal solution.
DATETIME | Stores a date/time value in the format of 'YYYY-MM-DD HH:MM:SS.ffffff'. When you only need derivatives of the value such as just the date, or just the time, there are helpers built into MySQL to aid in this.
