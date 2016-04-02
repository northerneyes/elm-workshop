Getting Started
===============

## Installation

1. Install [Node.js](http://nodejs.org) 4.0.0 or higher

2. Add an [editor plugin](http://elm-lang.org/install#syntax-highlighting) for your editor of choice.

3. Not required, but **highly** recommended: [install elm-format](https://github.com/avh4/elm-format#installation-) and integrate it into your editor so that it runs on save.

4. Run the following command to install everything else:

```bash
npm install -g elm@0.16.0 elm-live@2.0.4 elm-test@0.16.1-alpha3 elm-css@0.4.0
```

This command could take several minutes to complete.

## Clone this repository

Run this at the terminal:

```bash
git clone https://github.com/rtfeldman/elm-workshop.git
cd elm-workshop
```

## Create a GitHub Personal Access Token

We'll be using GitHub's Search API, and authenticated API access lets us experiment without worrying about the default rate limit. Since we'll only be accessesing
the Search API, these steps can be done either on your personal GitHub account or on a throwaway account created for this workshop; either way will work just as well.

1. Visit https://github.com/settings/tokens/new
2. Enter "Elm Workshop" under "Token description" and leave everything else blank.
3. Create the token and copy it into a new file called `Auth.elm`:

*Auth.elm*

```elm
module Auth (token) where


token =
  -- Your token should go here instead of this sample token:
  "abcdef1234567890abcdef1234567890abcdef12"
```

*Note:* Auth.elm is in `.gitignore` to avoid accidentally checking in an API
secret.

## Start with Part 1

Run this at the terminal:

```bash
cd part1
```

Now head over to the [README for Part 1](https://github.com/rtfeldman/elm-workshop/tree/master/part1)!
