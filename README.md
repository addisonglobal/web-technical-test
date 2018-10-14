# Addison Global Web Technical Assesement

## Introduction

Welcome to Addison Global Web Tech test.

The primary goal of this exercise is to assess how you reason about your ability to write clean, well tested and reusable code. There's no hard rules or tricky questions.

**We hope you have fun.**

## Glossary

* Promotion - A sports or casino offering with a purpose of encouraging potential customers to sign up.

## Brief

For this exercise you are required to build a fasst, responsive, mobile first promotions page. This promotions page consists of two views or filters:
* New Customers - a list of promotions only applicable to new customers
* All Promotions - a list of all promotions

When the page loads, you should fetch the data to render the promotions. The promotions object contains a flag `onlyNewCustomers` which indicates whether a promotion is only applicable to new customers or not.

Promotions must be sorted according to the `sequence` property.

## Data

We've provided an endpoint that can be accessed using the following URL:
<a href="http://www.mocky.io/v2/5bc3b9cc30000012007586b7" target="_blank">http://www.mocky.io/v2/5bc3b9cc30000012007586b7</a>

You can also find a sample of the data [data.json](data.json)

### Types

```js
/** The response type of the API call */
type ResponseType = PromotionType[];

/** Promotion Entity */
type PromotionType = {
    id: string,
    name: string,
    description: string,
    heroImageUrl: string,
    onlyNewCustomers: bool,
    termsAndConditionsButtonText: string,
    joinNowButtonText: string,
    sequence: number
};
```

## Technology

At Addison Global, we're big fans of React and Redux and, as such, we encourage you to solve the task in this stack. Despite this, you are free to use any technology or framework of your choosing.

## Screens

The provided screens are a wireframe, not a final design for the application. You are expected to implement the user interface by yourself. The use of component libraries might make this easier for you and is encouraged.

### New Customers Promotions

![New Customers Promotions](img/new-customers-promotions.png "New Customers Promotions")

### All Promotions

![All Promotions](img/all-promotions.png "All Promotions")

## The Deliverable

* A bundled/archived repository showing your commit history or a link to an accessible private repository with your work in (Github can host private repositories at a cost; there is no charge for doing so with Bitbucket). Git example for sending us a standalone bundle:

        git bundle create <yourname>.bundle --all --branches

* A Readme.md file explaining the decisions you've made solving this task including technology and library choices.
* Any instructions required to run your solution and tests in a Linux environment.
