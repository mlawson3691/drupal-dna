# AJAX and Testing Practice

##### Epicodus Drupal Code Review 4

#### By Mark Lawson

## Description

This simple application has two main features. First, articles are viewable on the front page using AJAX by way of a custom module. Second, a simple form accepts a single strand of DNA nucleotides and returns its matching strand. This application uses the Simpletest module for unit and funcitonal testing.

## Setup

* Clone this repository
* Set document root to the top level directory of the repository
* Import the database, called "dna", found in `sites/db-backup`
* Create a user for the database: username = "dna", password = "dna"
* Point browser to localhost
* Site maintenance account info: username = "dna", password = "dna"

## Specifications

* The application will return the correct letter based on input.
    * Example Input: 'A'
    * Example Output: 'T'

    * Example Input: 'T'
    * Example Output: 'A'

    * Example Input: 'G'
    * Example Output: 'C'

    * Example Input: 'C'
    * Example Output: 'G'

* The application will handle multiple characters.
    * Example Input: 'ATGC'
    * Example Output: 'TACG'

* The application will handle lowercase characters.
    * Example Input: 'atCG'
    * Example Output: 'TAGC'

* The application will return an error if anything other than A, T, C, and G is entered
    * Example Input: 'dog'
    * Example Output: 'You may only enter A, T, C, and G.'
